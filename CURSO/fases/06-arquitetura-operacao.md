# Fase 06 — Arquitetura, cloud e resposta a incidentes

**Semanas:** 43–50 · **Carga estimada:** 96 horas. Avance por domínio real, não automaticamente por data.

## Por que esta fase existe
Projetar serviços que operem com carga, falhas parciais e limitações de custo.

## Conhecimentos a dominar
processos/threads, concorrência/async, redes DNS/TLS, cache, filas, arquitetura monólito/modular, eventos, bounded contexts, SLA/SLO, logs/metrics/traces, p50/p95, rate limit, retries/backoff, circuit breaker, custo cloud, backup/restore, ADR, postmortem.

## Sprints semanais
| Semana | Tema | Entrega verificável |
|---|---|---|
| 43 | Sistemas operacionais e rede | Traçar jornada DNS→TLS→HTTP→processo→resposta. |
| 44 | Concorrência e filas | Simular trabalho paralelo sem duplicar pedidos. |
| 45 | Arquitetura e ADR | Comparar monólito modular e microsserviços para produto pequeno. |
| 46 | Observabilidade | Criar logs úteis, métrica de erro/latência e correlação. |
| 47 | Desempenho | Encontrar N+1 e comparar medições antes/depois. |
| 48 | Resiliência e recuperação | Projetar retry e timeout sem efeitos duplicados. |
| 49 | Incidente 404 | Investigar bug secreto com evidências e plano de correção. |
| 50 | On-call simulado | Postmortem sem culpabilização e apresentação em inglês. |

## Projeto de aplicação
Incidente 404, manutenção de uma codebase desconhecida.

## Gate obrigatório para prosseguir
Reproduzir, diagnosticar e corrigir defeito com regressão, métricas e trade-off explicados; elaborar postmortem.

## Inglês no trabalho
outage, root cause, impact, remediation, incident, observability, latency.

## Referências
[Google SRE book (referência)](https://sre.google/books/)

## Prova de autonomia
Resolver tarefa inédita sem IA (N0/N1), escrever casos-limite e registrar link de evidência, revisão e lição aprendida. Ver [rubrica](../AVALIACAO.md).

## Lição do mentor
Antes de mostrar sintaxe: perguntar o que é entrada, o que se transforma, que decisões existem, o que pode dar errado e como validar. Em seguida, exigir justificativa das escolhas técnicas.
