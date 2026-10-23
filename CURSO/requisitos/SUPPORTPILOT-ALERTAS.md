# SupportPilot — proposta de acompanhamento de prazos e qualidade (Ticket 006)

> Proposta oriunda de uma atividade educacional simulada em 23/10/2026. **Não foi implementada, testada nem implantada.** O aluno forneceu a ideia, e o mentor IA documentou refinamentos; não confundir com experiência profissional contratada.

## Necessidade levantada

O cliente recebeu resposta para a cobrança, mas continua sem acesso à conta. O prazo estimado de 48 horas para recuperar o acesso expirou. Precisamos manter o cliente informado e evitar que chamados abertos por muito tempo sejam esquecidos.

## Solução sugerida pelo aluno

1. Comunicar ao cliente que o acesso continua em andamento e que a equipe trabalha na solução.
2. Manter o ticket de acesso aberto, preservando o histórico e sem encerrar o atendimento geral.
3. Depois de **72 horas** de ticket aberto, gerar um **registro interno** para acompanhamento e qualidade do atendimento (QA).
4. Usar os dados agregados desses registros para entender causas de atrasos e melhorar processos e suporte.

## Refinamento discutido pelo mentor

- **48 horas (estimativa vencida):** enviar atualização ao cliente e avisar responsável ou supervisor conforme política. Não esperar 72 horas para fazer o primeiro aviso.
- **72 horas (limiar de investigação):** se o ticket continua aberto, abrir **um único alerta interno de acompanhamento**, associado ao ticket original, para análise e escalonamento. Não criar outro ticket externo do mesmo problema.
- **Depois:** atualizar o mesmo alerta interno enquanto o problema persistir. Um agendamento repetido não deve gerar alertas duplicados.
- **Quando resolver:** concluir o ticket de acesso; marcar o atendimento principal como resolvido apenas quando todas as pendências e condições necessárias estiverem satisfeitas; documentar encerramento do alerta de QA.
- **Proteção de dados:** o relatório de QA deve usar o mínimo de informações necessárias, sem copiar credenciais, informações sensíveis nem detalhes de pagamento indiscriminadamente.
- **Métricas:** atraso por categoria/equipe, duração até a resolução, frequência de exceder estimativas, motivos confirmados e recorrência. Medir antes de concluir que o atendimento melhorou.

## Regras para os estados (exemplo)

| Elemento | Antes do limite | Após limite / alerta | Após resolução |
|---|---|---|---|
| Ticket Financeiro | Resolvido | Resolvido | Resolvido |
| Ticket Acesso | Em andamento | Em andamento (atrasado) | Resolvido |
| Atendimento principal | Parcialmente resolvido | Parcialmente resolvido | Resolvido |
| Alerta QA | Ausente | Aberto (interno) | Concluído após revisão |

**Atrasado** é uma condição adicional, e não substitui necessariamente o estado **Em andamento**.

## Questões a decidir antes de escrever código

- 48 e 72 horas são **corridas ou úteis**? A partir da criação, da atribuição ou da última atualização?
- Qual nível de urgência e quais serviços exigem prazos diferentes?
- De quanto em quanto tempo o cliente deve receber atualizações significativas?
- Quem recebe o alerta interno e quem assume a revisão?
- Como o sistema detecta a passagem do prazo e evita duplicatas se a mesma verificação rodar duas vezes?
- O que fazer se ticket estiver aguardando uma resposta do próprio cliente?

## Primeiro critério verificável para a futura implementação

**Dado** um ticket de Acesso em andamento há mais de 72 horas corridas (valor provisório), **quando** a rotina de monitoramento for executada, **então** deve existir exatamente **um** alerta de QA interno vinculado ao ticket; executar a rotina novamente **não deve criar alertas repetidos**.

**Dado** um prazo estimado vencido e um ticket ainda não resolvido, **quando** a condição de atraso for identificada, **então** deve ser registrada uma atualização de status apropriada, com comunicação ao cliente conforme as regras e os contatos disponíveis.

Os requisitos ainda precisam ser refinados e aprovados. Não afirmar que o sistema envia alertas hoje.

## Competência estudada

- Separação entre comunicação externa e acompanhamento interno.
- Estado de ticket versus sinalização de atraso.
- Introdução a **eventos, prazos, alertas, observabilidade e regras de negócio**.
- Consideração futura de automação idempotente, autorização e escalonamento.

## Atualização — Central de alertas (Ticket 007)

O aluno propôs uma página interna com três grupos:

| Lista | O que significa |
|---|---|
| **Abertos** | Alertas ainda não assumidos, ordenados por prioridade e tempo |
| **Em andamento** | Um membro da equipe está investigando a ocorrência |
| **Concluídos** | Investigação interna encerrada com resultado documentado |

**Regra de unicidade proposta:** para uma mesma ocorrência de atraso de um ticket, abrir um único alerta de QA. Quando o monitor executar novamente, consultar o registro existente e, se houver um, **não criar nem reiniciar outro alerta**. A regra deve ser garantida no backend/banco, inclusive sob execução simultânea, e não apenas na tela.

**Diferença entre estados:** ticket do cliente e alerta de QA são entidades separadas; concluir revisão interna não significa necessariamente que o problema do cliente foi resolvido.

**Questões futuras:** decidir se um novo atraso depois de resolução e reabertura representa nova ocorrência e, portanto, pode gerar um novo alerta; determinar responsável, histórico, prioridades e acesso autorizado.

**Critérios verificáveis futuros:**
- O mesmo ticket e a mesma ocorrência de atraso, monitorados duas vezes, não criam dois alertas.
- O alerta em andamento continua em andamento após nova verificação.
- Uma ocorrência nova e legítima não fica invisível por conta de alerta antigo já concluído.
- A ordenação considera prioridades definidas e tempo sem atualização conforme política aprovada.

[Registro do Ticket 007](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2#issuecomment-6368187865).

## Próxima atividade

**Agora vamos sair do desenho da página e escrever a primeira regra executável em palavras.** O aluno deve explicar em três etapas: o que verificar ao detectar um ticket atrasado, quando criar e quando manter o alerta. Depois veremos um pequeno exemplo de código. O conceito de idempotência foi apresentado, mas ainda não demonstrado por código/teste.

Relato do aluno registrado na [Issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2).
