# DEV FORGE Labs — Manual do colaborador (simulação educacional)

> **AVISO:** a DEV FORGE Labs é uma empresa fictícia usada para aprendizagem. Contrato, salário, benefícios, colegas, promoções e experiência de trabalho descritos nesta pasta **não existem fora da simulação**. O aluno NÃO deve se apresentar a empregadores como funcionário dessa empresa. Os produtos, commits, projetos e competências reais do aluno, porém, podem compor seu portfólio com indicação clara de projeto educacional.

## Sua contratação fictícia

- **Cargo de entrada:** Junior AI Application Engineer (Engenheiro Júnior de Aplicações de IA).
- **Equipe:** Intelligent Products Engineering.
- **Regime fictício:** CLT, trabalho remoto no Brasil, com práticas de colaboração em inglês.
- **Salário fictício:** R$ 6.500 brutos/mês; benefícios inventados: R$ 900/mês de alimentação, plano de saúde e odontológico, equipamento corporativo, mentoria sênior e treinamento de inglês.
- **Referência:** faixa salarial júnior pode variar muito; exemplo escolhido como narrativa, não promessa ou dado de folha real. Em pesquisa de outubro de 2026, Glassdoor mostrava salário-base aproximado de R$ 4–9 mil para engenheiro júnior de IA no Brasil. Ver https://www.glassdoor.com.br/Sal%C3%A1rios/engenheiro-junior-inteligencia-artificial-sal%C3%A1rio-SRCH_KO0,41.htm .
- **Entrada no universo do curso:** Dia 1 de onboarding; sem competência reconhecida por antecipação.

## Quem é quem na empresa (todos fictícios)

- **Daniel Martins — Senior Software Engineer / Tech Lead:** mentor e revisor. Ensina, faz perguntas, divide problemas, evita resposta pronta, revisa PRs e define desafios inéditos de acordo com o progresso.
- **Laura Costa — Product Manager:** explica os problemas dos clientes e ajusta prioridades; ensina a fazer perguntas antes de implementar.
- **Marina Ribeiro — QA Engineer:** cria casos difíceis, cobra evidências, investiga erros e regressões.
- **Alex Chen — AI Engineer:** orienta LLMs, RAG, avaliações, tool calling, riscos e custos; participa depois que os fundamentos estiverem firmes.
- **Você — Junior AI Application Engineer:** investiga e explica, implementa incrementalmente, registra descobertas, testa e responde pela qualidade dos artefatos.

O mentor ChatGPT pode interpretar os personagens, deixando sempre claro quando está em simulação. O aluno pode sair do personagem e pedir explicação técnica em português a qualquer momento.

## O que a profissão faz na vida real?

AI Application Engineers trabalham com programação, APIs, integração de modelos de IA, regras de negócio, tratamento e proteção de dados, qualidade, avaliação, custos, infraestrutura e manutenção. O trabalho não é somente escrever prompts. É saber quando NÃO usar IA também.

Papéis parecidos: Junior AI Engineer, Generative AI Engineer, AI Automation Engineer, Software Engineer (AI Applications), Agent Engineer. Esses títulos variam por empresa, setor e nível.

## Produto principal da empresa-escola: SupportPilot

Imagine um SaaS usado por empresas que recebe mensagens de clientes. Precisamos criar um produto que **entenda a solicitação, classifique corretamente, busque informações permitidas e ajude um atendente**, sem inventar respostas e sem executar mudanças sensíveis sem aprovação.

Evolução conforme habilidade comprovada:

1. **Dia 1 — No-code:** descobrir o que o cliente pediu, qual equipe atende e onde estão as ambiguidades. Entrada → regra → saída. Sem sintaxe.
2. **Primeira semana:** discutir regras, exemplos e situações que exigem perguntar antes de decidir.
3. **Primeiros programas:** construir um classificador por regras simples em Python e criar testes.
4. **Versionamento e equipe:** abrir issues, branches e PRs e aprender a explicar o que mudou.
5. **Aplicativo web:** interface acessível para receber e acompanhar mensagens.
6. **Backend e dados:** API, banco relacional, autenticação, limites de acesso e histórico.
7. **Qualidade e operação:** CI/CD, logs, métricas, simulação de erros e rollback.
8. **IA aplicada:** usar LLM e recuperação de documentos (RAG), comparar com baseline determinístico e medir erros, latência e custos.
9. **Agentes:** usar ferramentas somente com autorizações, auditoria e confirmação humana.
10. **Apresentação final:** demonstrar o produto, explicar arquitetura em inglês e responder perguntas de um entrevistador.

**Projetos do currículo existente** (CorteJusto, OficinaOS, DocPilot, OpsPilot e demais) continuam válidos como contratos paralelos da empresa-escola e peças de portfólio. A narrativa serve para conectar os fundamentos, não eliminar projetos.

## Como funciona um expediente didático

Cada sessão representa um período de trabalho, mesmo que o aluno só estude 20 minutos:

1. **Daily / check-in (2 min):** o sênior pergunta o que você entendeu e o que está bloqueando.
2. **Ticket (problema concreto):** a gerente de produto descreve o usuário, a necessidade, as restrições e o que comprova sucesso.
3. **Pair work (explicação e tentativa):** o sênior orienta um conceito, demonstra um pequeno exemplo e propõe UM desafio novo.
4. **Work / entrega:** o aluno resolve com seu raciocínio, depois usa editor/código quando chegar a hora.
5. **Review (análise e feedback):** QA e sênior questionam as escolhas, mostram consequências e pedem uma melhoria pontual.
6. **Stand-up in English (inglês gradual):** começa com uma expressão; evolui até discussão de PR e reunião técnica.
7. **Work log (registro):** a atividade, evidência, ajuda de IA, entendimento e próxima tarefa vão para o GitHub; o aluno pode salvar primeiro no chat e registrar depois.

**Não avançar por calendário ou dramatização.** A aprovação depende da avaliação e de evidências rastreáveis. Simular salário e benefícios não cria competência, emprego real ou certificado.

## Como o sênior deverá ensinar

- Nunca partir de termos como "invariante" ou "pseudocódigo" sem ensino prévio.
- Tradução humana → exemplo resolvido → uma pergunta por vez → feedback → conceito técnico → inglês técnico.
- Antes de ensinar tecnologia, mostrar **qual problema concreto ela resolve**.
- Quando o aluno disser "não entendi", diminuir a carga, identificar precisamente o obstáculo e apresentar outro exemplo, não aumentar o número de exercícios.
- O sênior **não deve sempre concordar**. Ele precisa mostrar os erros com respeito, cobrar compreensão, consequências e segurança.
- Nas primeiras sessões o aluno pode responder diretamente pelo chat. GitHub serve como registro posterior. Código e PRs são introduzidos gradualmente.
- A IA não deve fingir simular processos reais (deploy, execução de testes ou aprovação) sem evidência.

## Semanas e avaliações

O [roadmap principal](ROADMAP.md) permanece válido: 72 semanas estimadas a 12h/semana, com avanço por competência. O papel fictício e a rotina profissional evoluem, mas não garantem contratação e não devem ser registrados como emprego formal no currículo.

## Como retomar em outro chat

Abra [HANDOFF.md](HANDOFF.md), [PROGRESSO.md](PROGRESSO.md), este manual e a [tarefa atual](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2). O tutor deverá retomar a cena e o problema sem presumir a resposta.

**Situação inicial canônica:** você acabou de ser apresentado ao time e Daniel vai explicar para que serve o SupportPilot. Nenhum desafio ainda foi aprovado.
