# ADR-001 — Primeira estratégia de triagem do SupportPilot
**Status:** proposta aceita para detalhamento, **ainda não implementada nem validada**  
**Origem:** exercício educacional da DEV FORGE Labs, ticket #2, 23/10/2026  
**Contexto:** empresa, equipe e cenário são simulados. A proposta e a revisão foram desenvolvidas em conversa de aprendizagem, não em emprego real.

## Contexto

Uma mensagem de cliente pode conter múltiplos assuntos, porém **cada ticket pode pertencer a somente um departamento**. O negócio quer que o cliente acompanhe um atendimento unificado. A primeira versão precisa ser planejada para **duas semanas** e orçamento limitado.

## Alternativas apresentadas pelo aprendiz

1. Triagem humana: atendente lê a mensagem e direciona problemas.
2. Agente de IA: classifica mensagens livres e sugere/gera os encaminhamentos.
3. Questionário de categorias: cliente marca vários motivos de contato, descreve caso não listado e sistema cria tickets correspondentes.

O aprendiz identificou a operação comum de classificação/encaminhamento e, na decisão seguinte, recomendou combinar **questionário + atendimento humano**, deixando o uso de IA para uma etapa posterior.

## Proposta para o MVP

- Formulário com **categorias prioritárias** (ex.: cobrança duplicada, login), seleção múltipla e campo “Outro problema”.
- Sistema recebe a seleção e cria **um caso/atendimento-pai**, com tickets filhos independentes, cada um atribuído a apenas uma equipe.
- Cliente acompanha todos os tickets ligados ao caso em um **único lugar**.
- Pedidos ambíguos, sensíveis ou não contemplados seguem para **revisão humana**.
- Acesso de cada departamento fica limitado aos dados necessários, sem compartilhamento irrestrito de informações de cobrança ou conta.
- Manter confirmação para evitar tickets duplicados por reenvio do formulário (conceito a ser explicado nas fases posteriores).

## Por que essa escolha?

- Triagem por formulário tem menor complexidade técnica inicial e comportamento previsível.
- Revisão humana preserva julgamento nos casos que fogem às regras.
- Um agente de IA seria uma camada posterior, apenas se evidência mostrar valor em relação a custos, riscos e ganho de cobertura.
- Começar com uma lista **pequena e útil** é mais viável do que tentar mapear todas as possíveis solicitações em duas semanas.

## Hipóteses a validar

**A afirmação de que o filtro resolveria 99% das situações não é evidência.** O protótipo precisa distinguir:
- **Taxa de encaminhamento correto:** percentual de solicitações enviadas à equipe adequada;
- **Taxa de cobertura do formulário:** percentual das solicitações que cabem nas categorias atuais;
- **Taxa de revisão humana:** casos que exigem exceção;
- **Resolução efetiva:** percentual de solicitações efetivamente resolvidas, que depende das equipes e não apenas do filtro;
- **Tempo de resolução** e satisfação do cliente, se houver dados representativos.

Nenhuma dessas métricas foi aferida neste exercício.

## Decisões ainda não tomadas

- Como o atendimento-pai deve se comportar quando um ticket-filho está resolvido e outro atrasado?
- Qual informação cada equipe pode visualizar?
- O que o cliente deve receber: uma confirmação inicial, atualizações parciais e/ou uma resposta consolidada?
- Como impedir geração repetida de tickets?
- Quais categorias são realmente prioritárias no piloto?

## O que foi avaliado

**Demonstração inicial:** capacidade de comparar três abordagens, reconhecer restrições de prazo e custo, propor solução híbrida sem IA desnecessária e modelar um caso contendo múltiplos tickets.

**Não demonstrado ainda:** implementação, testes, segurança, medição operacional, entendimento profundo de arquitetura ou implantação. A mentoria é simulada; não equivale a experiência profissional contratada.

## Próximo exercício (uma pergunta)

O Financeiro resolveu o ticket da cobrança, mas a equipe de Acesso ainda não conseguiu resolver o problema de login. **O que o cliente deve ver ou receber enquanto espera, considerando que tem um único atendimento principal?** Explique por quê.

## Inglês técnico
- **MVP (Minimum Viable Product):** produto mínimo viável.
- **Ticket routing:** encaminhamento de chamados.
- **Human review / human-in-the-loop:** revisão ou intervenção humana.
- **Parent case / child tickets:** atendimento principal / tickets relacionados.
- **Trade-off:** escolha que troca uma vantagem por outra.
