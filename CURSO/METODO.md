# Método pedagógico: laboratório de engenharia

## A arquitetura de aprendizagem
**Compreender → Prever → Construir → Quebrar → Corrigir → Explicar → Generalizar.**

Cada semana produz:
1. Documento do problema, stakeholders, regras e restrições.
2. Antes de programar: pseudocódigo/diagrama e 3+ testes previstos.
3. Implementação pequena e executável.
4. Testes automatizados quando apropriado e teste manual documentado.
5. Registro das falhas, hipótese, evidência e correção.
6. PR com resumo, testes e riscos; revisão simulada de pares.
7. Demonstração técnica de 2–5 minutos ou texto equivalente em inglês.

## Política de IA de quatro níveis
- **N0 — Sem IA:** raciocínio, prova de fundamentos, solução inicial e entrevista.
- **N1 — IA socrática:** IA só pergunta e dá pistas; aprendiz constrói a resposta.
- **N2 — Copiloto:** IA pode explicar, sugerir testes e discutir design; toda linha aceita deve ser compreendida.
- **N3 — Engenharia assistida:** IA gera partes do código, mas o aprendiz especifica, revisa, testa, integra e responde por elas.

Uma entrega informa nível usado, ferramenta, sugestões aceitas/rejeitadas e como a solução foi verificada. Nenhuma aprovação é dada a artefato que não pode ser explicado sem IA. Segurança, privacidade e direitos autorais prevalecem.

## Revisão por pares simulada
Professor/assistente revisa como sênior exigente: pergunta "por quê?", aponta cenários ausentes e não oferece solução completa antes da tentativa do aluno. Nas etapas finais, revisar PRs de terceiros e participar de projeto open source é recomendado.

## Regra de realidade
Cada projeto tem personagens fictícios, demanda realista, limite de prazo, dados de exemplo, alteração inesperada e incidente introduzido. Nada de projetos "to-do" que passam sem autenticação, erros, logs, testes ou documentação.

## Mudança de requisitos
A cada sprint haverá uma alteração de escopo. O aprendiz cria ADR (Architecture Decision Record) curto: contexto, alternativas, decisão e consequências.

## Como provar autonomia
Explicar uma decisão sem ler o código; implementar um ajuste novo com IA N0/N1; depurar um defeito introduzido; responder perguntas sobre custo, segurança e risco.

## Template de sessão
- O que preciso entender?
- O que sei/pressuponho?
- Qual é a evidência?
- Quais entradas, saídas e invariantes?
- Como descubro se errei?
- Como explicaria isso a uma pessoa do time em inglês?
- Qual aprendizado registrarei no GitHub?
