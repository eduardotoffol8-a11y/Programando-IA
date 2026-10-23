# GitHub como currículo técnico: plano de evidências

> Documento vivo do DEV FORGE AI. Objetivo: transformar aprendizado e projetos em competências demonstráveis para vagas de Junior Software Engineer e AI Application Engineer no Brasil e no exterior. Nunca inflar domínio ou experiência.

## 1. A diferença entre projeto, portfólio e experiência

- **Projeto**: algo foi construído.
- **Portfólio**: é possível entender, executar, testar e avaliar o que foi construído.
- **Evidência profissional**: o candidato consegue explicar requisitos, decisões, trade-offs, alterações, resultados, limitações e sua contribuição, inclusive sem assistência de IA.
- **Experiência profissional formal**: vínculo, clientes ou trabalho remunerado real, quando existirem. Projeto pessoal não deve ser anunciado como emprego.

O GitHub amplia um currículo de uma página; não o substitui integralmente.

## 2. Estrutura de apresentação (vitrine em 60 segundos)

1. Criar repositório **público** com nome EXATAMENTE igual ao login de usuário `eduardotoffol8-a11y`, contendo `README.md` na raiz. Assim o GitHub mostra a apresentação no perfil.
2. Bio objetiva: **Aspiring Software Engineer | Building practical full-stack and AI applications | Python • TypeScript • APIs**. Ajustar para habilidades comprovadas; não declarar especialista antecipadamente.
3. Destacar 3 a 5 projetos, escolhidos por relevância para a vaga. GitHub permite fixar até 6.
4. Cada destaque: problema real, captura/demonstração, stack verificada, decisões, testes, como executar, limitações, contribuição própria.
5. Disponibilizar resumo curto também em inglês, e links para um currículo tradicional e LinkedIn somente quando existirem.

## 3. Matriz de prova por competência

| Competência | Evidência pública e auditável | Prova oral/prática |
| --- | --- | --- |
| Lógica e algoritmos | exercícios próprios, casos-limite, testes automatizados | resolver requisito surpresa e explicar invariantes |
| Git e colaboração | issues, branches, commits claros e pull requests pequenos | explicar diff, conflitos e revisar um PR |
| Backend e APIs | endpoints, contratos, erros HTTP, testes de integração | explicar autenticação, fluxo e falhas |
| Banco de dados | schema, migrações, consultas e índices | justificar relacionamentos, transações e consultas |
| Frontend | aplicação acessível, responsiva, demo | reproduzir e corrigir um bug |
| Qualidade | CI, testes reprodutíveis, regressão | reproduzir erro e escrever teste antes da correção |
| Segurança | threat model, autorização, proteção de segredos | mostrar como impedir acesso cruzado de usuários |
| Operação | deploy, logs, runbook, plano de rollback | explicar incidente e recuperação |
| IA aplicada | RAG/agent com evals, falhas e métricas de custo/latência | provar que o sistema reconhece limites e lida com prompt injection |
| Comunicação | ADR, documentação, revisão, vídeo/pitch em inglês | defender decisões com clareza |

## 4. Dossiê obrigatório de cada projeto

Criar no projeto, conforme pertinência:
- `README.md`: o que resolve, para quem, demo e como rodar.
- `docs/PROBLEM.md`: contexto, restrições e critérios de aceite.
- `docs/ARCHITECTURE.md`: diagrama e responsabilidade de cada parte.
- `docs/DECISIONS/`: ADRs, opções consideradas, escolha e motivos.
- `docs/TESTING.md`: comandos verificáveis, cenários positivos/negativos e cobertura contextualizada.
- `docs/CASE_STUDY.md`: problema → investigação → decisão → implementação → resultado → aprendizado.
- Links para uma issue e uma PR com histórico legível e revisão.
- `docs/AI_USAGE.md`: trabalho da IA, decisão própria, como revisou e o que refez.
- `docs/LIMITATIONS.md`: falhas conhecidas, questões pendentes e próximos passos.
- Screenshot ou vídeo curto sem dados pessoais, preferindo demonstração executável.

**Regra de alegação:** nenhuma métrica de precisão, porcentagem de testes, usuários ou redução de tempo sem proveniência identificável. Um README não substitui execução e inspeção.

## 5. Projetos já existentes: diagnóstico inicial (22/10/2026)

- **Programando-IA**: repositório da formação, não prova suficiente sozinho. Manter progresso e links para produtos entregues.
- **FinAi**: README atual é sobretudo guia padrão de execução do AI Studio; reescrever como estudo de caso após auditoria técnica.
- **spam-scam**: README contém texto de modelo Markdown e percentuais de acurácia; limpar formatação e conferir métricas com scripts, dataset e metodologia reproduzíveis.
- **cortecloud-site**: README padrão de Next.js; descrever função real do software e contribuição.
- **Evolua**: repositório privado, possível fonte de estudos de caso. Não publicar código, dados de usuários, credenciais ou arquitetura sensível sem análise explícita.

### Exemplo de evidência real para ESTUDAR (não copiar como alegação de autoria)

O PR #75 do Evolua, **Atualizar automaticamente as PWAs sem interromper treinos** (17/10/2026), está mesclado no repositório privado. A descrição relata problema de atualização adiada, mudança no ciclo de atualização, regressões e vários testes. É uma boa base para uma futura entrevista **somente depois** de estudar a implementação, reexecutar/verificar os testes e declarar com honestidade o que foi executado por você e o que foi gerado/implementado com IA.

Modelo de explicação:
- Problema: atualizações pendentes em sessão longa.
- Restrições: não interromper treino e preservar dados.
- Hipóteses: ciclo de vida da PWA, atualização de service worker, cache e estados.
- Solução: explicar o diff real, em vez de recitar o texto do PR.
- Validação: executar testes, demonstrar antes/depois e discutir o rollback.

## 6. Método de demonstração em entrevistas

Use a estrutura **P-D-V-R-A**:
1. **Problema**: o que estava quebrado/ausente, para quem.
2. **Decisão**: alternativas consideradas e por que uma venceu.
3. **Validação**: testes, riscos e medições verificáveis.
4. **Resultado**: entrega observável, com limites.
5. **Aprendizado**: o que faria de outra maneira.

A entrevista deve incluir exercício novo, leitura de código desconhecido, debugging de falha, desenho de API/SQL e explicação oral em inglês. Evidências devem ser coerentes com o domínio demonstrado, não substituí-lo.

## 7. Transparência sobre inteligência artificial

Em todo projeto expressivo:
- Registrar o que você definiu: requisitos, critérios de aceite, política de segurança e escolhas técnicas.
- Registrar o que a IA sugeriu ou implementou.
- Registrar como inspecionou, testou, corrigiu e assumiu responsabilidade pelo resultado.
- Ser capaz de reconstruir um componente pequeno do zero, localizar falha e revisar um patch sem IA.

Evitar dizer “desenvolvi sozinho” quando houve assistência decisiva. Isso **não desqualifica** o trabalho; aumenta a credibilidade sobre seu papel real.

## 8. Plano incremental de 90 dias (marcos por entrega, não por calendário rígido)

**Dias 1–15**
- Criar README do perfil com posicionamento honesto PT/EN.
- Identificar três projetos candidatos e escolher um para auditoria.
- Adicionar README específico, screenshots seguras e comandos reproduzíveis ao primeiro projeto.

**Dias 16–30**
- Reproduzir a execução e testes do projeto escolhido.
- Abrir 2–3 issues de melhorias, implementar uma correção delimitada em PR.
- Registrar causa raiz e evidências.

**Dias 31–60**
- Criar o primeiro projeto curricular de raiz (CorteJusto) com testes próprios.
- Praticar Git por PRs e defender cada mudança verbalmente.
- Apresentar 3 minutos em inglês sobre problema, decisões, testes e limitações.

**Dias 61–90**
- Evoluir a aplicação para API e persistência simples conforme competências alcançadas.
- Adicionar CI e demonstração segura.
- Revisar currículo, README e uma simulação de entrevista.
- Priorizar maturidade do software em vez de abrir muitos repositórios.

## 9. Portas de prontidão para candidaturas

**Gate A — Fundamentos:** resolver caso novo sem IA, escrever testes, explicar estrutura de dados e depurar falha.

**Gate B — Engenharia de software:** entregar frontend/backend ou API/SQL com segurança, CI, operação e documentação, em PR auditável.

**Gate C — AI Application Engineer:** integrar LLM/RAG/agente com avaliações, segurança, latência/custo e explicar os modos de falha.

A aprovação depende das rubricas em `AVALIACAO.md`. Nenhum gate garante uma vaga; cada um aumenta a preparação demonstrável.

## 10. Links oficiais

- https://docs.github.com/pt/account-and-profile/tutorials/using-your-github-profile-to-enhance-your-resume
- https://docs.github.com/pt/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- https://docs.github.com/pt/account-and-profile/how-tos/profile-customization/pinning-items-to-your-profile

**Data do diagnóstico:** 22/10/2026. Revalidar antes de aplicar para vagas.
