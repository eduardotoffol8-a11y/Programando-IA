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

## Próxima atividade

Antes de codificar, perguntar ao aluno: **“Se o sistema verificar o mesmo ticket atrasado de hora em hora, o que deve fazer para não criar dezenas de alertas iguais?”**. O conceito de idempotência deve ser ensinado de modo simples após a tentativa.

Relato do aluno registrado na [Issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2).
