# Fase 07 — AI Engineering: LLMs, retrieval e avaliação

**Semanas:** 51–58 · **Carga estimada:** 96 horas. Avance por domínio real, não automaticamente por data.

## Por que esta fase existe
Projetar sistemas com modelos de linguagem que produzam respostas verificáveis, seguras e com custo administrável.

## Conhecimentos a dominar
ML conceitual, treinamento vs inferência, estatística de métricas, tokens, contexto, temperatura, structured outputs, embeddings, chunking, busca lexical/semântica/híbrida, RAG, citations, grounding, abstenção, privacy, prompt injection, offline evals, latency/cost.

## Sprints semanais
| Semana | Tema | Entrega verificável |
|---|---|---|
| 51 | Modelos e estatística básica | Separar IA probabilística de algoritmo determinístico; métricas. |
| 52 | API LLM e contratos | Solicitar saída estruturada e validar schema. |
| 53 | Embeddings e busca | Comparar lexical, vetorial e híbrida em perguntas anotadas. |
| 54 | Ingestão e chunking | Versionar corpus sintético e registrar origem dos trechos. |
| 55 | Pipeline RAG | Responder com citações ou abster-se. |
| 56 | Dataset de avaliação | Anotar ≥50 perguntas, negativas, confusas e conflitantes. |
| 57 | Segurança e custos | Executar testes de injeção e registrar p50/p95/custo. |
| 58 | DocPilot release | Publicar relatórios de qualidade e falhas conhecidas. |

## Projeto de aplicação
DocPilot com benchmark reproduzível e controle de permissões.

## Gate obrigatório para prosseguir
Provar por dados que mudança melhorou (ou piorou) qualidade e custo; demonstração de abstenção, isolamento e defesas.

## Inglês no trabalho
retrieval, ground truth, precision, recall, hallucination, evaluation, latency, context window.

## Referências
[OpenAI API docs](https://platform.openai.com/docs)

## Prova de autonomia
Resolver tarefa inédita sem IA (N0/N1), escrever casos-limite e registrar link de evidência, revisão e lição aprendida. Ver [rubrica](../AVALIACAO.md).

## Lição do mentor
Antes de mostrar sintaxe: perguntar o que é entrada, o que se transforma, que decisões existem, o que pode dar errado e como validar. Em seguida, exigir justificativa das escolhas técnicas.
