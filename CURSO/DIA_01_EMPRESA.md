# Dia 01 — Seu primeiro dia como Junior AI Application Engineer

> **Tudo nesta cena é fictício.** O exercício é real e produz competências transferíveis. Você não precisa de computador, editor ou GitHub para participar: pode responder no chat com o mentor.

## Bem-vindo à DEV FORGE Labs

**Cargo fictício:** Junior AI Application Engineer  
**Salário fictício:** R$ 6.500 brutos mensais + R$ 900 de vale alimentação, benefícios e trabalho remoto (ver [manual da empresa](EMPRESA_SIMULADA.md)).  
**Gestor fictício:** Daniel Martins, Senior Software Engineer.  
**Seu ponto de partida real:** iniciante absoluto em lógica e engenharia de software.

### Mensagem do mentor

> Bom dia! Sou Daniel. Não vou pedir que você programe algo que nunca viu. Nosso objetivo hoje é conhecer o produto e entender o que significa transformar um problema em instruções precisas. Se qualquer palavra não fizer sentido, interrompa e me pergunte. Sua pergunta é parte do trabalho.

## Produto que vamos construir com o tempo

O **SupportPilot** ajuda um time de atendimento a lidar com mensagens de clientes. Ele deve saber qual equipe pode ajudar, quando faltam informações e, mais tarde, como usar IA para responder com fontes e permissões. Hoje vamos começar apenas com um problema de encaminhamento.

### Regras iniciais combinadas com Laura (Product Manager)

Nossa empresa tem três equipes:

| Equipe | O que resolve | Exemplo de solicitação |
|---|---|---|
| **Acesso** | Entrar na conta e recuperar acesso | “Não consigo fazer login” |
| **Financeiro** | Pagamento, cobrança e reembolso | “O sistema cobrou duas vezes” |
| **Planos** | Mudança ou cancelamento do plano | “Quero trocar de plano” |

**Regra de segurança:** se a mensagem não for clara, não inventar uma decisão. Encaminhar para análise de uma pessoa ou pedir esclarecimento, conforme o procedimento vigente.

## Antes do desafio, veja Daniel resolver um exemplo

**Mensagem do cliente (entrada/input):** “Meu cartão foi cobrado duas vezes.”

**Pensamento do desenvolvedor:** é problema de cobrança. Qual das três equipes resolve cobranças? A equipe Financeiro.

**Resultado (saída/output):** encaminhar para Financeiro.

Percebeu? Recebemos informação, aplicamos uma regra e escolhemos um resultado. Isso já é o coração da lógica de programação.

### Sua primeira tarefa, uma pergunta por vez

**Mensagem do cliente:** “Troquei de celular e não consigo entrar na minha conta.”

**Pergunta de Daniel:** para qual equipe você encaminharia esta mensagem: **Acesso**, **Financeiro**, **Planos** ou **revisão humana**? Explique com suas palavras o detalhe da mensagem que levou à decisão.

**Envie a resposta no chat. Não faça mais nada por enquanto.** O mentor deve revisar a explicação antes da tarefa seguinte.

### Depois que responder

Daniel discutirá:
1. Como identificar as informações importantes na mensagem.
2. O que pode dar errado se o sistema fizer uma suposição.
3. Como escrever regras que sejam consistentes.
4. Gradualmente, quando fazer classificação por regras e quando integrar um modelo de IA.

**Inglês do dia:** `customer message` = mensagem do cliente; `support team` = equipe de suporte; `route` = encaminhar. Reconhecer essas expressões já é suficiente no primeiro encontro.

## Como registrar a experiência

Depois de compreender e receber revisão, documente a tentativa em `CURSO/evidencias/eduardo/dia-01-supportpilot.md` ou, se for aluno externo, em seu repositório pessoal. Você pode usar [o modelo de registro](templates/MODELO_DIA_01_EMPRESA.md).

- Problema apresentado, em suas palavras.
- Equipe escolhida e justificativa.
- Feedback e o que aprendeu.
- Uma expressão em inglês.
- Link da evidência, quando salvo.

A tarefa do GitHub [Issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2) acompanha este onboarding. **Não marque aprovação sem revisão.**

## Saída do primeiro dia

Você só precisa demonstrar que entende: **mensagem recebida → regra de negócio → decisão explicada**, e que sabe identificar quando o sistema não deve adivinhar.

Mais tarde teremos testes adversariais, código, Git, API e agentes de IA. **Hoje é uma única decisão bem justificada.**
