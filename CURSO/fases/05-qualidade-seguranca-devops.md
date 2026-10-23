# Fase 05 — Qualidade, segurança e entrega contínua

**Semanas:** 35–42 · **Carga estimada:** 96 horas. Avance por domínio real, não automaticamente por data.

## Por que esta fase existe
Software útil precisa resistir a entradas ruins, mudanças e operações reais.

## Conhecimentos a dominar
test pyramid, unit/integration/e2e, mocks, fixtures, CI GitHub Actions, coverage sem fetiche, TDD, code quality, OWASP, threat modeling, secrets, dependency scanning, Docker/Compose, environments, deployment, rollback, monitoring.

## Sprints semanais
| Semana | Tema | Entrega verificável |
|---|---|---|
| 35 | Testes e estratégia | Cobrir requisitos críticos e falhas, não só happy path. |
| 36 | CI e PR | Rodar linter/testes automaticamente e bloquear merge com falha. |
| 37 | Threat modeling | Mapear superfícies e implementar correções necessárias. |
| 38 | Segredos e hardening | Remover token fictício vazado e documentar revogação. |
| 39 | Docker e ambientes | Reproduzir stack sem configuração manual frágil. |
| 40 | Deploy e rollback | Publicar staging, simular falha e voltar versão. |
| 41 | Testes de regressão | Reproduzir bug de autorização e escrever teste de prevenção. |
| 42 | Release profissional | OficinaOS 1.0, changelog, runbook, auditoria de PR. |

## Projeto de aplicação
OficinaOS operacional no ambiente de demonstração; nenhum dado real.

## Gate obrigatório para prosseguir
CI verde, teste de autorização, nenhum segredo, instalação reproduzível e rollback executável documentado.

## Inglês no trabalho
test suite, CI pipeline, vulnerability, environment variable, rollback, release notes.

## Referências
[OWASP Top Ten](https://owasp.org/www-project-top-ten/) · [GitHub Actions](https://docs.github.com/en/actions) · [Docker](https://docs.docker.com/)

## Prova de autonomia
Resolver tarefa inédita sem IA (N0/N1), escrever casos-limite e registrar link de evidência, revisão e lição aprendida. Ver [rubrica](../AVALIACAO.md).

## Lição do mentor
Antes de mostrar sintaxe: perguntar o que é entrada, o que se transforma, que decisões existem, o que pode dar errado e como validar. Em seguida, exigir justificativa das escolhas técnicas.
