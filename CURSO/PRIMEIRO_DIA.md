# Primeiro dia: roteiro de 30–60 minutos, sem escrever código

**Objetivo:** você terminará este roteiro entendendo onde fica o curso, qual é sua tarefa atual, onde escreverá suas respostas e como me enviará o resultado para revisão.

**Você precisa somente de:** conta no GitHub, navegador no celular ou computador, conexão à internet e bloco de notas (opcional). **Não precisa instalar Python, VS Code, Docker, pagar serviços ou saber inglês ainda.**

> No celular, nomes e posições de menus podem variar no navegador/app. Se não vir os botões, tente pelo navegador em “Site para computador”. Não execute comandos desconhecidos nem compartilhe tokens.

## Você, dono do curso: roteiro direto para Eduardo

### Passo 1 — Entrar na escola

1. Acesse [o repositório Programando-IA](https://github.com/eduardotoffol8-a11y/Programando-IA).
2. Faça login no GitHub caso seja solicitado.
3. A página inicial possui um arquivo chamado **README.md**: é a entrada principal.
4. Clique em **CURSO** e depois em **PRIMEIRO_DIA.md**; você já está lendo o guia certo.

**Resultado esperado:** você consegue localizar a pasta `CURSO/` no repositório.

### Passo 2 — Ver o que precisa fazer

1. Abra [a Aula 001](aulas/001-pensamento-computacional.md).
2. Leia o cenário da marcenaria e a regra para a quantidade de portas.
3. Abra [a Issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2).
4. Entenda a diferença: **a aula ensina e explica; a issue é a ordem de serviço com o que será avaliado**.

**Resultado esperado:** você sabe dizer, numa frase, qual problema deve resolver.

### Passo 3 — Preparar sua primeira entrega

1. Abra o [Modelo de Entrega da Aula 001](templates/MODELO_ENTREGA_001.md).
2. Leia as seções. Ele já contém os espaços para completar, **mas não o gabarito**.
3. Você pode redigir primeiro num bloco de notas. Não poste senha, CPF, dados de clientes nem outras informações privadas.
4. Seu arquivo final se chamará `aula-001-resposta.md`.

### Passo 4 — Criar o arquivo no GitHub (sem terminal)

Este passo salva sua resposta no GitHub de modo que sobreviva ao chat.

1. Volte ao [repositório principal](https://github.com/eduardotoffol8-a11y/Programando-IA) e abra a aba **Code** (Código).
2. Clique **Add file → Create new file** (Adicionar arquivo → Criar arquivo). Se estiver no celular e o botão não aparecer, use a visualização de computador do navegador.
3. No campo do nome, digite exatamente:
   `CURSO/evidencias/eduardo/aula-001-resposta.md`
   O GitHub usa as barras para criar as pastas necessárias.
4. Copie o texto do [modelo](templates/MODELO_ENTREGA_001.md) para o editor. Preencha aos poucos; você não precisa resolver tudo numa única sessão.
5. Clique **Commit changes…** e confirme com uma mensagem como `docs: inicio minha solucao da aula 001`.
6. Para editar depois, abra o arquivo e use o ícone de lápis **Edit this file**, altere e salve com novo commit.

**Resultado esperado:** o navegador abre uma página com seu arquivo `aula-001-resposta.md`, com um link próprio.

> Para o PRIMEIRO exercício escrito, editar na branch principal é aceitável porque é apenas seu arquivo Markdown pessoal. Nas fases de programação, utilizaremos branches e pull requests para revisar mudanças de código.

### Passo 5 — Fazer o exercício de verdade

Leia a aula e complete no arquivo, com seu próprio raciocínio:

- Qual é a entrada? O que é uma entrada inválida?
- Qual é a saída? Qual informação é devolvida em caso de erro?
- Como um funcionário extremamente literal decidiria entre 1, 2 e 3 portas?
- O que deve acontecer exatamente em 60, 120 e 300 cm?
- Que testes mostram que a regra é segura e previsível?
- O que muda se acima de 240 cm exigir revisão humana?
- Como você explicaria o problema em inglês simples?

**Importante:** você pode pedir ao mentor explicações e pistas, mas precisa tentar primeiro. Não precisa saber ponto e vírgula nem programar.

### Passo 6 — Entregar para revisão

1. Abra a página do arquivo que você acabou de salvar.
2. Copie a URL da barra de endereços.
3. Abra a [Issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2).
4. Em **Leave a comment / Add a comment**, escreva:
   
   ```text
   Minha entrega da Aula 001:
   [COLE AQUI O LINK DO MEU ARQUIVO]

   Maior dificuldade:
   [UMA DÚVIDA REAL]

   Nível de ajuda de IA usado:
   [N0, N1, N2 ou N3]
   ```
5. Clique **Comment** para enviar o comentário. Depois me envie o link da issue ou do arquivo nesta conversa ou em outra.

**Resultado esperado:** existe um arquivo salvo, um link de entrega e uma tarefa à espera de revisão.

### Passo 7 — Receber feedback, corrigir e registrar progresso

- O mentor confere a entrega, pede justificativas e cria alguns casos novos para ver se você entendeu.
- Você corrige o arquivo, se necessário, fazendo outro commit.
- **Somente depois da aprovação** atualizamos [PROGRESSO.md](PROGRESSO.md) com o link de evidência e o próximo passo.
- A conclusão depende da compreensão, não só de uma caixa marcada.

## Se você for um futuro aluno e não for o dono deste repositório

Não tente editar o repositório original, pois você provavelmente não terá permissão. Seu trabalho deve ficar **na sua própria conta**.

**Caminho mais simples:**
1. Faça login em [github.com](https://github.com).
2. Clique no ícone **+ → New repository** ou acesse `https://github.com/new`.
3. Nome sugerido: `minha-jornada-dev-forge-ai`; escolha público (para portfólio) ou privado (para maior privacidade).
4. Marque **Add a README file** e conclua em **Create repository**.
5. Dentro **do seu novo repositório**, use **Add file → Create new file**.
6. Nomeie o arquivo como `aulas/aula-001-resposta.md`.
7. Use [o modelo de resposta](templates/MODELO_ENTREGA_001.md), preencha e salve em **Commit changes**.
8. Envie o link desse arquivo ao seu mentor ou ao canal de revisão escolhido pela turma; **não registre entregas pessoais na issue #2 do autor sem convite**.
9. Mantenha um `PROGRESSO.md` no seu próprio repositório; pode usar [o modelo de diário](templates/MODELO_PROGRESSO_ALUNO.md).

> Não copie ou redistribua integralmente o conteúdo das aulas em um projeto público: o curso ainda não possui licença de redistribuição definida. O repositório pessoal deve conter **seu trabalho original e links para as aulas**.

## Como saber que terminou o primeiro dia?

- [ ] Encontrei o README e a pasta CURSO.
- [ ] Abri a primeira aula e a tarefa correspondente.
- [ ] Sei qual é meu espaço pessoal de trabalho.
- [ ] Criei e salvei uma primeira versão de resposta.
- [ ] Sei como gerar e enviar o link ao mentor.
- [ ] Sei que ainda preciso de revisão para concluir a aula.

Se algo falhar, diga **em qual passo parou e o que aparece na tela**. Seu mentor deve orientar esse clique antes de continuar com conteúdo técnico.

## Depois do primeiro dia

Leia [Como funciona uma atividade](COMO_FUNCIONA_UMA_ATIVIDADE.md), continue a primeira aula e só então pense em ferramentas para programar: [Ambiente de trabalho](AMBIENTE.md).
