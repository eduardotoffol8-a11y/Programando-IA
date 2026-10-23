# Desafio opcional da Aula 001 — aprofundamento posterior

> **AVISO PARA INICIANTES:** este não é o exercício da primeira aula. Faça primeiro [Aula 001 simplificada](../aulas/001-pensamento-computacional.md), receba feedback e avance gradualmente. Aqui há perguntas que pertencem a uma revisão posterior sobre limites, tipos, testes e alterações de requisitos.

# Material original de aprofundamento

> **Antes de começar:** este é seu primeiro contato com o curso? Siga [o tutorial do primeiro dia](../PRIMEIRO_DIA.md). Você resolverá esta atividade **em um arquivo escrito**, não no editor de programação. Copie o [modelo de resposta](../templates/MODELO_ENTREGA_001.md), preencha e [entregue conforme o roteiro](../PRIMEIRO_DIA.md#passo-6--entregar-para-revisão). A [issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2) reúne os critérios de avaliação.

**Fase:** 00 · **Duração:** 90–120 minutos · **Modo inicial:** N0 (sem IA para resolver). **Nenhuma linguagem de programação exigida.**

## Cenário realista
Uma pequena marcenaria recebe pedidos de armários. O vendedor precisa sugerir **quantidade inicial** de portas para um vão de largura informada pelo cliente. É apenas uma regra de orçamento didática; não substitui dimensionamento estrutural ou cálculo real de ferragens.

### Regra contratada pelo cliente fictício
- O campo `largura_cm` deve ser numérico e maior que zero e no máximo 300 cm.
- Se largura ≤ 60 cm → 1 porta.
- Se 60 cm < largura ≤ 120 cm → 2 portas.
- Se 120 cm < largura ≤ 300 cm → 3 portas.
- Caso contrário → erro claro, **sem recomendar quantidade**.
- A entrada sempre está em centímetros; não aceitar unidade implícita.
- Não arredondar a medida para decidir a faixa. `60.01` não é `60`.

## O que significa programar aqui?
Transformar regras de linguagem humana num procedimento que:
1. Recebe uma entrada.
2. Verifica se a entrada pertence ao domínio válido.
3. Compara a entrada com limites em ordem.
4. Produz uma saída inequívoca.
5. Garante invariantes: para largura válida, exatamente uma opção; para inválida, nenhuma.

## Exercício A — Prever sem executar
Copie uma tabela e complete a coluna "saída esperada" para:
`-1`, `0`, `1`, `59.99`, `60`, `60.01`, `119.99`, `120`, `120.01`, `299.99`, `300`, `300.01`, `"abc"` e `null`.
Explique 3 limites, inclusive a diferença entre "menor que" e "menor ou igual".

## Exercício B — Pseudocódigo humano
Escreva instruções que um funcionário literal seguiria sem usar termos vagos ("normal", "grande", "mais ou menos"). Não escreva Python. Indique o que acontece se o valor vier vazio, negativo, em texto ou fora do intervalo.

## Exercício C — Faça seu próprio teste adversarial
Crie mais 5 entradas inéditas que poderiam revelar erro. Em pelo menos uma, discuta diferença entre `120`, `120.0` e `120.001`. Descreva unidade e precisão.

## Exercício D — Requisito muda
Cliente informa que larguras acima de 240 cm devem exigir **análise humana**, sem sugestão automática. Atualize o algoritmo e a tabela. Mostre qual regra anterior deixou de valer. Não implemente antes de esclarecer se o valor 240 está incluído.

## Exercício E — Explique para um colega dos EUA
Escreva 60–100 palavras em inglês descrevendo os inputs, os branches, o error handling e um edge case. Pode consultar glossário de termos, mas a lógica é sua.

## Entrega
Arquivo `aula-001-resposta.md` contendo:
- Definição do problema, entrada e saída.
- Regras e domínio de validade.
- Pseudocódigo.
- Tabela de pelo menos 14 casos.
- 5 testes inéditos.
- Mudança de requisito e impacto.
- Explicação em inglês.
- Autoavaliação: ponto de dúvida mais importante.

## Critérios de aceite
- Nenhuma medida inválida gera número de portas.
- Os limites 60, 120 e 300 são tratados exatamente.
- Nova regra de 240 é aplicada de modo coerente.
- Pseudocódigo encerra e é determinístico para cada entrada válida.
- Explicação em português demonstra domínio; inglês é praticado, não precisa ser perfeito.

## Pergunta de profundidade
Um programa pode executar todas as instruções e ainda assim estar errado? Explique diferença entre **bug de implementação**, **erro na especificação** e **regra comercial mal definida**.

## Não olhe o gabarito primeiro
Mentor deve questionar e dar pistas, não entregar resposta pronta. A avaliação deve incluir 3 casos inéditos criados na hora.

