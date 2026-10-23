# English for Developers: inglês incorporado ao trabalho

## Roteiro por fase
- 00–01: nouns, verbs e explicação de problema, inputs/outputs, conditions, loops.
- 02–03: GitHub issues, PR description, bug reports, review comments e async messages.
- 04–05: APIs, databases, logs, tests, incidents, security.
- 06–07: architecture decisions, trade-offs, cloud, LLM evaluations.
- 08–09: technical interviews, system design, demos, negotiation e incident postmortem.

## Ritual semanal (20–30 min em 3 dias)
1. Ler 1 seção de documentação em inglês e parafrasear em português.
2. Criar glossário técnico com definição e exemplo próprios.
3. Explicar 1 decisão do projeto em inglês escrito (80–150 palavras).
4. Ensaiar 2 minutos de stand-up em inglês: Yesterday / Today / Blockers.
5. Ao fechar PR, informar What changed? Why? How was it tested? Risks?

## Frases reais de equipe
- "I reproduced the bug with these steps."
- "The root cause appears to be a missing validation."
- "I chose this design because it keeps the API backward compatible."
- "This trade-off improves latency but increases infrastructure cost."
- "Could you clarify the expected behavior for invalid inputs?"
- "I rolled back the deployment after monitoring the error rate."

## Glossário inicial
requirement = requisito; acceptance criteria = critérios de aceite; edge case = caso-limite; invariant = propriedade que deve continuar verdadeira; trade-off = escolha com benefícios e custos; debugging = investigação de defeito; pull request = proposta de alteração; code review = revisão de código; regression = defeito em algo que funcionava; deployment = disponibilização; rollback = reversão; throughput = volume processado por tempo; latency = demora de resposta; idempotency = repetição que preserva o efeito; observability = entender o sistema por sinais internos; hallucination = resposta não sustentada do modelo; retrieval = busca de informações; evaluation = medição da qualidade; prompt injection = tentativa de mudar instruções por conteúdo não confiável.

## Simulados de entrevista
1. "Walk me through a project you built."
2. "How do you approach an ambiguous requirement?"
3. "Tell me about a production-like incident you debugged."
4. "What is the difference between frontend and backend?"
5. "How do you validate an API request?"
6. "When would you use an index in a database?"
7. "Explain a trade-off you made."
8. "How do you avoid exposing secrets?"
9. "How did you measure the quality of your AI feature?"
10. "What would you do if a model called the wrong tool?"

## Aferição
Início: explicar o próprio projeto com apoio. Intermediário: defender PR e responder follow-ups. Final: simular reunião técnica e entrevista de 30–45 min, registrar falhas e treinar novamente. Fluência não é pressuposta nem automática.
