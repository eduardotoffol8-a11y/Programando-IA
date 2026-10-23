# Aula 001 — Seu primeiro raciocínio de programador

> **Nova apresentação principal do curso:** [Dia 01 como Junior AI Application Engineer](../DIA_01_EMPRESA.md). Este exercício de marcenaria continua disponível como **prática complementar** da mesma lógica (informação → regra → resultado), para quem desejar outro exemplo. Não é a tarefa inicial obrigatória do onboarding.

**Nível:** iniciante absoluto • **Tempo sugerido:** 15–25 minutos • **Precisa saber programar? NÃO.** • **Ferramenta:** este texto e uma resposta em português.

> **Comece por aqui.** Você não precisa entender GitHub, inglês técnico, testes automáticos ou comandos para fazer esta atividade. **Pode responder diretamente ao seu mentor no chat.** Quando entendermos juntos, você poderá guardar sua resposta no GitHub usando [este modelo simples](../templates/MODELO_ENTREGA_001.md). O [guia do primeiro dia](../PRIMEIRO_DIA.md) explica os cliques.
>
> **Objetivo único da aula:** aprender que um computador recebe uma informação, segue uma regra clara e apresenta um resultado.

## 1. Imagine que você está ensinando um funcionário novo

Uma marcenaria fictícia quer sugerir uma quantidade inicial de portas usando somente a largura informada pelo cliente.

O cliente da oficina estabelece as seguintes regras **inventadas apenas para aprender** (não são recomendações técnicas reais):

| Largura informada pelo cliente | Quantidade que o funcionário deve indicar |
| --- | --- |
| De mais de 0 até 60 centímetros | 1 porta |
| Maior que 60 até 120 centímetros | 2 portas |
| Maior que 120 até 300 centímetros | 3 portas |
| Zero, número negativo ou maior que 300 | Avisar que a medida não é aceita |

**Até 60** inclui 60. **Maior que 60** não inclui 60. A gente estudará esse detalhe com calma.

### Um exemplo feito junto

O cliente diz: **“Meu vão tem 90 centímetros.”**

- A largura é maior que zero? **Sim.**
- Está na primeira faixa, até 60 cm? **Não.**
- Está na segunda faixa, acima de 60 e até 120 cm? **Sim.**
- Então a resposta segundo a regra é **2 portas**.

Não tivemos que escrever uma linha de programação: **tomamos uma decisão seguindo instruções claras.**

## 2. Três palavras novas, em linguagem humana

- **Entrada (input):** a informação que chega. Aqui, a largura de 90 cm.
- **Regra (rule):** o que deve ser feito com essa informação. Aqui, comparar a largura com as faixas.
- **Saída (output):** a resposta dada após aplicar a regra. Aqui, 2 portas.

O caminho é: **cliente informa a largura → aplicamos a regra → indicamos a quantidade de portas**.

Um **algoritmo** é um modo organizado de descrever os passos necessários para resolver um problema. Por enquanto, isso basta.

## 3. Seu EXERCÍCIO 1: descubra a resposta

**O que fazer:** leia a tabela de regras no começo da aula e complete apenas a coluna que está vazia. Não precisa copiar o código, criar aplicativo nem desenhar nada.

O primeiro exemplo já está preenchido:

| Largura | Sua resposta |
| --- | --- |
| 90 cm | **2 portas** (exemplo resolvido) |
| 45 cm | **?** |
| 110 cm | **?** |
| 135 cm | **?** |

**Como responder no chat:** `45 = ___; 110 = ___; 135 = ___`.

Seu objetivo não é decorar números. É mostrar qual regra foi escolhida em cada caso.

## 4. Seu EXERCÍCIO 2: explique UMA decisão

Uma pessoa pede um armário com **120 cm de largura**.

**Pergunta:** pela regra, devemos indicar 2 ou 3 portas? Por quê?

**Dica:** repare na diferença entre **“até 120 cm”** e **“maior que 120 cm”**.

Responda com **uma frase em português**, da sua maneira. Não precisa de palavras técnicas.

## 5. Seu EXERCÍCIO 3: e se a informação estiver errada?

O cliente informa largura de **0 cm**.

O funcionário deveria escolher 1, 2 ou 3 portas? Ou deveria informar que a medida não é válida?

**Explique em uma frase** usando a regra inicial.

É assim que começamos a aprender a não deixar o sistema fornecer uma resposta ruim quando recebe informação ruim.

## 6. Como entregar sem se perder

**Agora:** envie somente as respostas aos exercícios 1, 2 e 3 na conversa com o mentor. Pode ser assim:

```text
Exercício 1:
45 = ...
110 = ...
135 = ...

Exercício 2:
Em 120 cm, eu escolheria ... porque ...

Exercício 3:
Com 0 cm, o sistema deveria ... porque ...

Minha dúvida:
...
```

**Depois que a lógica estiver clara:** para manter seu aprendizado registrado, preencha [o arquivo-modelo simplificado](../templates/MODELO_ENTREGA_001.md) e salve seguindo o [roteiro do primeiro dia](../PRIMEIRO_DIA.md). No curso piloto de Eduardo, o destino é `CURSO/evidencias/eduardo/aula-001-resposta.md`. Outros alunos usam repositório próprio.

**Você não precisa resolver tudo em uma sessão.** Se não entender uma pergunta, envie somente o que tentou e diga onde travou. O mentor deve explicar esse ponto, não entregar outra lista de termos.

## 7. Como saber que você entendeu?

Você consegue:
- Identificar a informação que o sistema recebeu.
- Aplicar a regra certa para uma largura informada.
- Explicar por que escolheu aquele resultado.
- Reconhecer que uma medida inválida não deve gerar uma resposta inventada.

Quando conseguir fazer isso com exemplos inéditos, podemos avançar. **Nenhuma exigência de inglês avançado, pseudocódigo, planilhas de 14 casos ou cinco testes extras nesta primeira atividade.**

### Um pouquinho de inglês, sem cobrança

- **Input** = informação que entra.
- **Rule** = regra.
- **Output** = resposta que sai.

Frase para reconhecer, não precisa decorar agora: **“The input is the width.”** (A informação de entrada é a largura.)

## Próxima aula ou desafio

Depois da revisão, aprenderemos como escrever um conjunto de instruções sem ambiguidades, testar medidas exatamente nos limites e explicar o que fazer quando o cliente muda de ideia. Os [desafios aprofundados da antiga versão](../desafios/001-aprofundamento-opcional.md) foram preservados, mas **não fazem parte da primeira entrega**.
