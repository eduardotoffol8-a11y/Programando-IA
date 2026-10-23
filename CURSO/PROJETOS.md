# Produtos-âncora: projetos reais, progressivos e verificáveis

**Nunca são apenas tutoriais.** Cada projeto inclui história de cliente fictício, backlog, decisões, testes, bugs semeados, métricas e demonstração para alguém que não conhece o código.

## P1 — CorteJusto | Motor de orçamento de marcenaria
**Problema:** escritório perde tempo com cálculos inconsistentes de chapas, peças, desperdício e orçamento.
**Entrega:** biblioteca/CLI em Python para validar medidas e calcular peças, custos e preço conforme regras configuráveis.
**Casos obrigatórios:** milímetros vs centímetros, arredondamento explícito, medida ausente, preço negativo, espessura, peça fora da chapa, descontos e histórico de versões das regras.
**Métrica:** 100% dos casos de aceitação passam; erro de cálculo zero na suíte definida; invariantes explicadas.
**Mudança inesperada:** fornecedor troca espessura ou preço no meio do orçamento.
**Skills:** decomposição, decisão, funções, testes, imutabilidade de regras e debugging.

## P2 — OficinaOS | Sistema de ordens de serviço
**Problema:** acompanhar cliente, pedido, peças, pagamentos e status com rastreabilidade.
**Entrega:** frontend acessível em TypeScript; backend em Python/FastAPI; PostgreSQL; autenticação/autorização; migrations; CI; deploy de demonstração.
**Casos obrigatórios:** cadastro/edição, filtros, transições de status permitidas, idempotência de operações críticas, paginação, erro de rede, 2 perfis de acesso, histórico de auditoria.
**Métricas:** contratos de API testados, pipeline verde, zero segredos, guia de operação.
**Mudança inesperada:** clientes passam a poder visualizar pedidos sem editar custos internos.
**Skills:** arquitetura web, SQL, segurança, testes e Git/PR.

## P3 — Incidente 404 | Laboratório de manutenção
**Problema:** um sistema entregue por outra equipe degrada em horário de pico.
**Entrega:** fork ou codebase de treinamento com bug reproduzido, issue técnica, logs, hipóteses, correção mínima, teste de regressão e postmortem em inglês.
**Cenários:** consulta N+1, validação ausente, erro de fuso horário, endpoint lento, falha de integração; primeiro diagnosticar, só depois consertar.
**Métricas:** tempo de diagnóstico documentado; teste que falha antes e passa depois; rollback descrito.
**Skills:** manutenção, observabilidade, performance, comunicação de incidente.

## P4 — DocPilot | Assistente de conhecimento verificável (RAG)
**Problema:** equipe consulta 100+ documentos e precisa de respostas com fontes e limite de confiança.
**Entrega:** ingestão, busca híbrida ou semântica conforme comparação, retrieval, citação de fontes, regra de abstenção, API, UI simples, logs de custo/latência.
**Dados:** documentos criados para o exercício com permissões e conflitos controlados; não usar documentos privados.
**Métricas:** conjunto de ≥50 perguntas anotadas, acerto de resposta, fidelidade de citação, abstenção correta, custo por pergunta e latência p50/p95.
**Mudança inesperada:** documento desatualizado contradiz outro e usuário sem acesso tenta consultar.
**Skills:** LLM, embeddings, RAG, avaliação, privacidade e reliability.

## P5 — OpsPilot | Agente com ferramentas e supervisão
**Problema:** triagem de tickets solicita ações em sistemas simulados.
**Entrega:** agente com leitura de tickets, classificação, busca em base, proposta de resposta e criação controlada de tarefas (tool calling), autorização e trilha de auditoria.
**Casos obrigatórios:** dry-run, confirmação humana antes de escrever, ferramentas com escopo mínimo, 2 ataques de prompt injection, erro/timeout, compensação de execução parcial, deduplicação e orçamento de chamadas.
**Métricas:** ≥60 cenários de avaliação incluindo negativos; nenhuma ação sensível sem aprovação; taxa de sucesso, falso positivo, custo e tempo registrados.
**Mudança inesperada:** documento malicioso pede exportação de dados; agente deve rejeitar.
**Skills:** agentic systems, tool design, orquestração, estados, avaliação e segurança.

## P6 — Capstone profissional | Cliente de verdade, dados seguros
Escolher problema real com permissão explícita, ou reproduzir cenário de empresa com personas e datasets sintéticos. Entregar discovery, especificação, ADRs, código, testes, CI/CD, monitoramento, runbook, deploy, demo, pitch e relatório de trade-offs. Projeto deve comprovar competências da vaga-alvo, não apenas incorporar IA.

## Artefatos mínimos por projeto
`README.md`, `REQUIREMENTS.md`, `ARCHITECTURE.md`, `THREAT_MODEL.md`, `TEST_PLAN.md`, `RUNBOOK.md`, `DECISIONS/`, `EVALS/` (se IA), issues e PRs. Não criar documentos vazios por burocracia; incluir decisões úteis.

O Evolua real pode fornecer temas e cenários *sem* copiar dados, credenciais ou lógica proprietária ao material público.
