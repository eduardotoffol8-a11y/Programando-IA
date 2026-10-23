# Mapa da escola: onde você estuda, trabalha, entrega e acompanha tudo

> **Se nunca utilizou o GitHub, comece por [PRIMEIRO_DIA.md](PRIMEIRO_DIA.md).** Este guia explica os lugares e o significado das palavras, não exige programação.

## Visão rápida em português simples

O DEV FORGE AI funciona como uma **empresa-escola de engenharia de software**, com ambientes diferentes para funções diferentes.

| Lugar | Pense nele como… | O que você faz | Link ou localização |
|---|---|---|---|
| **Repositório Programando-IA** | Biblioteca e secretaria da escola | Lê a trilha, as aulas, os projetos e os critérios | [Abrir repositório](https://github.com/eduardotoffol8-a11y/Programando-IA) |
| **Pasta `CURSO/aulas/`** | Sala de aula | Lê explicação, situação realista e exercícios | [Aula 001](aulas/001-pensamento-computacional.md) |
| **Issues** | Quadro de tarefas da empresa | Descobre o que precisa entregar, tira dúvidas e acompanha avaliação | [Primeira tarefa, issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2) |
| **Seu repositório / pasta de evidências** | Mesa de trabalho + caderno de laboratório | Guarda respostas, arquivos e projetos que VOCÊ criou | [Como criar](PRIMEIRO_DIA.md) |
| **GitHub editor web / VS Code / Codespaces** | Oficina de trabalho | Escreve Markdown no início; escreve e executa código nas fases seguintes | [Escolher ambiente](AMBIENTE.md) |
| **Pull Requests (PRs)** | Mesa de revisão de colegas | Propõe mudanças e recebe comentários antes de incorporar trabalho | [Fluxo das atividades](COMO_FUNCIONA_UMA_ATIVIDADE.md) |
| **PROGRESSO.md** | Boletim e diário de evolução | Registra evidências verificadas, dúvidas e próxima tarefa | [Progresso do curso piloto](PROGRESSO.md) |
| **ChatGPT / mentor** | Professor + revisor técnico | Esclarece raciocínio, faz perguntas, revisa entrega e propõe desafios novos | [Retomar em novo chat](HANDOFF.md) |

### Fluxo do trabalho

```text
1. ABRIR O CURSO
       ↓
2. LER A AULA (sala de aula)
       ↓
3. ENTENDER A ISSUE (tarefa)
       ↓
4. RESOLVER NO SEU ESPAÇO (mesa de trabalho)
       ↓
5. SALVAR E ENTREGAR O LINK (evidência)
       ↓
6. RECEBER REVISÃO + TESTE INÉDITO (avaliação)
       ↓
7. REGISTRAR PROGRESSO E AVANÇAR
```

**O GitHub não corrige automaticamente suas respostas.** Uma issue ou um commit comprova que houve entrega; entendimento e aprovação exigem revisão.

## Por que existem espaços diferentes?

- **Curso** não é um aplicativo. É o roteiro das aulas e desafios.
- **Ambiente de desenvolvimento** é o lugar para escrever e rodar código, seja no computador, seja num editor em nuvem quando disponível.
- **Repositório de trabalho** é o local onde fica o histórico público ou privado do que você realmente fez.
- **Portfólio** contém apenas projetos selecionados e bem documentados.
- **ChatGPT** ajuda a estudar, mas não substitui os arquivos de evidência persistidos no GitHub.

## Quem é você nesta escola?

O aprendiz começa como **trainee de desenvolvimento** em uma empresa fictícia chamada **DEV FORGE Labs**. Não se trata de contratação nem experiência empregatícia real. O projeto simula responsabilidades profissionais reais:

- **Cliente / Product Owner:** apresenta uma necessidade, uma urgência e critérios de aceitação.
- **Você / Developer:** investiga, decide, testa, constrói e explica.
- **Mentor / Tech Lead:** faz revisão crítica, pede justificativas e aponta riscos.
- **QA / Test Engineer:** tenta encontrar falhas e confirma os casos-limite.
- **Operações / SRE (mais adiante):** simula incidentes, logs, implantação e recuperação.

No começo, você só trabalha com raciocínio escrito. Depois trabalha com pequenos programas, APIs, bancos de dados e, por fim, agentes de IA.

## Onde guardo as minhas respostas?

**Piloto Eduardo (proprietário do repositório):** `CURSO/evidencias/eduardo/aula-001-resposta.md`, criado no primeiro dia. É uma pasta de exemplos e progresso pessoal, **não é gabarito**.

**Futuros estudantes:** cada pessoa usa seu próprio repositório GitHub para as evidências, com arquivos `aulas/aula-001-resposta.md`, `PROGRESSO.md` e projetos pessoais. O repositório principal permanece como material oficial. A política de licença e redistribuição ainda será definida; não publicar cópias integrais de aulas sem permissão.

**Privacidade:** evite dados privados, senhas, tokens, prints de clientes reais e informações sensíveis; todo arquivo num repositório público pode ser visto por outras pessoas. Um estudante pode optar por repositório privado, ciente de que o mentor precisa de acesso ou do trecho compartilhado para revisar.

## Vocabulário que você verá muito

| Palavra | Tradução prática | Exemplo |
|---|---|---|
| Repository / repo | Pasta de projeto com histórico | `Programando-IA` |
| README | Apresentação e instruções | “Leia isso primeiro” |
| Issue | Tarefa, dúvida ou problema registrado | “Criar lógica das portas” |
| Commit | Registro de uma alteração salva | “Adicionei tabela de testes” |
| Branch | Linha de trabalho separada | `aula-001-solucao` |
| Pull Request / PR | Pedido de revisão de alterações | “Revisem minha solução” |
| Review | Análise técnica da entrega | “Seu teste não cobre 120,01” |
| Test | Maneira de verificar comportamento | “Entrada 0 deve ser rejeitada” |
| Deployment / deploy | Publicação de uma aplicação | Site acessível na web |
| Debugging | Investigar e corrigir um defeito | Entender por que um cálculo erra |

## Links para continuar

1. [Primeiro dia: faça o passo a passo sem terminal](PRIMEIRO_DIA.md)
2. [Como funciona cada experiência profissional simulada](COMO_FUNCIONA_UMA_ATIVIDADE.md)
3. [Onde programar e quando instalar ferramentas](AMBIENTE.md)
4. [Como entregar a resposta da Aula 001](templates/MODELO_ENTREGA_001.md)
5. [Como pedir ajuda e continuar em outro chat](HANDOFF.md)
