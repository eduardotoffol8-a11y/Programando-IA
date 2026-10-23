# Fase 08 — Engenharia de agentes e orquestração

**Semanas:** 59–66 · **Carga estimada:** 96 horas. Avance por domínio real, não automaticamente por data.

## Por que esta fase existe
Agente útil é software com ações controladas, estado, ferramentas, métricas, limites e supervisão humana.

## Conhecimentos a dominar
tool/function calling, MCP conceitos, planner/executor, máquina de estados, filas e jobs, persistência, erros de ferramenta, idempotência, retries, approvals, least privilege, human-in-the-loop, prompt injection, audit trails, evals, custos e runbooks.

## Sprints semanais
| Semana | Tema | Entrega verificável |
|---|---|---|
| 59 | Ferramentas vs texto | Desenhar contrato de ferramentas com validação e permissões. |
| 60 | Máquina de estados | Especificar estados e transições do agente. |
| 61 | MCP e integrações | Explicar fronteiras de confiança; implementar mock de ferramenta. |
| 62 | Aprovação humana | Proibir escrita antes de confirmação e registrar consentimento. |
| 63 | Falha parcial e retry | Simular timeout, duplicidade e compensação. |
| 64 | Ataques e abuso | Red team de prompt injection e exfiltração simulada. |
| 65 | Evals do agente | Executar ≥60 cenários e medir sucesso, violação e custo. |
| 66 | OpsPilot release | Publicar demo com logs, dry-run, limites e runbook. |

## Projeto de aplicação
OpsPilot para tickets fictícios e integrações simuladas.

## Gate obrigatório para prosseguir
Demonstrar que nenhuma ação sensível ocorre sem aprovação, inclusive sob prompt injection; métricas e regressão automatizadas.

## Inglês no trabalho
tool calling, permission boundary, orchestration, state machine, approval, audit trail.

## Referências
[Model Context Protocol](https://modelcontextprotocol.io/) · [OWASP](https://owasp.org/)

## Prova de autonomia
Resolver tarefa inédita sem IA (N0/N1), escrever casos-limite e registrar link de evidência, revisão e lição aprendida. Ver [rubrica](../AVALIACAO.md).

## Lição do mentor
Antes de mostrar sintaxe: perguntar o que é entrada, o que se transforma, que decisões existem, o que pode dar errado e como validar. Em seguida, exigir justificativa das escolhas técnicas.
