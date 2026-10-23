# Ambiente de trabalho: onde você vai estudar e programar

> **Iniciante absoluto?** Não instale nada agora. Siga [o PRIMEIRO DIA](PRIMEIRO_DIA.md), que pode ser concluído pelo navegador. Veja também [o mapa da escola](MAPA_DA_ESCOLA.md).

## Resposta direta: onde vou colocar a mão na massa?

Nas primeiras aulas você não escreve código. Você **lê uma tarefa, escreve seu raciocínio em um arquivo Markdown no GitHub e envia o link para revisão**. Markdown é só um texto com uma formatação simples (`.md`), não uma linguagem de programação.

Mais adiante, ao programar de verdade, você terá opções:

| Opção | Onde abre? | Serve para quê? | Quando usar? |
|---|---|---|---|
| **GitHub no navegador** | github.com | Ler aula, editar texto Markdown, registrar trabalho e conversar por issues | **Agora, na Fase 00**, inclusive pelo celular |
| **VS Code** | Programa instalado em notebook/desktop | Escrever e executar programas, usar extensões e terminal | Ao chegar à Fase 01 |
| **GitHub Codespaces** | Ambiente de desenvolvimento em nuvem, aberto pelo GitHub (quando habilitado) | Usar editor e terminal sem instalar ferramentas localmente | Alternativa ao VS Code local, quando houver acesso/cota |
| **Terminal** | No VS Code local ou Codespaces | Executar comandos de programas, testes e Git | A partir da Fase 01, ensinado passo a passo |
| **Deploy de teste** | Hospedagem de aplicação, configurada mais adiante | Tornar uma aplicação acessível para verificação | A partir de web/backend, quando fizer sentido |

### Preciso de computador?

- **Hoje não:** o primeiro exercício é pensamento computacional por escrito, então celular ou notebook servem.
- **Para formação profissional completa:** **um computador com teclado será altamente recomendado** para programar, depurar e trabalhar com ferramentas reais. O celular pode acompanhar aulas e comentários, mas costuma tornar desenvolvimento e testes mais difíceis.
- **Quero evitar instalações:** uma opção em fases futuras é Codespaces, se sua conta e limites de uso permitirem. Não pressupor que é gratuito ou ilimitado; verificar cota, cobrança e configuração de cada conta antes de iniciar.

## Exemplo real da sua rotina por fase

### Fase 00 — Hoje: sala de aula e caderno digital
1. **Leia a aula**: [Aula 001](aulas/001-pensamento-computacional.md).
2. **Veja o pedido do cliente**: [issue #2](https://github.com/eduardotoffol8-a11y/Programando-IA/issues/2).
3. **Preencha seu arquivo**: [modelo da entrega](templates/MODELO_ENTREGA_001.md).
4. **Salve no GitHub**: tutorial [passos 3–4](PRIMEIRO_DIA.md).
5. **Entregue o link** e receba revisão.

**Exemplo de caminho do aluno piloto Eduardo:** `CURSO/evidencias/eduardo/aula-001-resposta.md`.

### Fases 01–02 — Oficina Python
**O que faremos:** abrir uma pasta de projeto, criar `calculo_portas.py`, escrever condições, executar, descobrir bugs e construir `test_calculo_portas.py`.

**Onde faremos:** VS Code no computador ou ambiente de nuvem adequado. O ambiente será configurado junto com a primeira aula de código, sem exigir instalações antecipadas.

**Como comprovaremos:** arquivo de código, comandos executados, testes, commits, issues e PRs.

### Fases 03–05 — Desenvolvimento profissional web
**O que faremos:** construir tela de usuário, API que recebe pedidos, banco de dados e autenticação usando projetos isolados do curso.

**Onde faremos:** editor, terminal, navegador com ferramentas de desenvolvedor, banco de dados de desenvolvimento e GitHub para revisão.

**Como comprovaremos:** aplicação executável, API testada, diagramas, testes automatizados e publicação de demonstração segura.

### Fases 06–09 — Ambiente de equipe e IA
**O que faremos:** diagnosticar incidentes, publicar aplicações, integrar modelos de IA, construir agentes com autorização de ferramentas, avaliar resultados e apresentar decisões em inglês.

**Onde faremos:** repositórios próprios dos projetos, ambientes de teste e serviços usados dentro de cotas e limites seguros.

**Como comprovaremos:** PRs, testes automatizados, casos de falha, documentação, demos e provas de domínio sem IA.

## Palavras que não deveriam assustar

- **Editor:** programa onde se escreve conteúdo ou código.
- **Terminal:** janela para dar instruções ao computador por texto; aprenderemos a usar, sem decorar comandos no início.
- **Python:** linguagem para expressar nossos algoritmos como programas executáveis.
- **Git:** registra a evolução do projeto e ajuda a recuperar versões.
- **GitHub:** site que hospeda repositórios Git, tarefas e revisões.
- **Codespace:** computador de desenvolvimento em nuvem com editor e terminal.
- **Commit:** gravação identificada de uma alteração no repositório.
- **PR:** pedido para revisar uma mudança proposta.

## Ferramentas recomendadas por fase (instalação adiada até necessário)

- Fase 00: somente navegador e GitHub.
- Fases 01–02: Python 3, Git, VS Code ou ambiente equivalente; testes com pytest.
- Fases 03–04: Node.js LTS, TypeScript, ferramentas HTTP, banco PostgreSQL.
- Fases 05–06: CI, Docker/Compose, deploy de testes, logs e rollback.
- Fases 07–08: integrações de IA com orçamento limitado ou modelos simulados (*mocks*) sem custo obrigatório.
- Fase 09: aplicações e demos sem credenciais ou dados privados.

## Regras de segurança e custo

Nunca publique tokens, senhas, chaves de API, cookies de sessão, dados pessoais ou dumps de produção. Não experimente diretamente em sistemas comerciais. Use dados fictícios, contas de teste e ambientes separados. Quando chegar a hora de usar serviços de nuvem, escolha e confirme antes o que pode gerar cobrança.

**Próximo passo:** [PRIMEIRO_DIA.md](PRIMEIRO_DIA.md).
