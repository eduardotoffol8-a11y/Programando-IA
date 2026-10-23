# Ambiente de trabalho progressivo

## Ferramentas recomendadas
- GitHub (Issues, Pull Requests, Actions) e Git.
- Editor de código como VS Code ou equivalente, com terminal.
- Python 3 e ambiente virtual; testes com pytest.
- Node.js LTS, TypeScript e testes adequados à aplicação.
- PostgreSQL; cliente SQL.
- Docker/Compose quando chegar à fase de infraestrutura.
- Ferramenta para requisições HTTP, logs e profiler.
- Ferramentas de IA opcionais, com política de dados e limites de gasto.

## Setup em camadas
**Fase 00:** navegador, editor e GitHub; nenhum serviço pago obrigatório.
**Fases 01–02:** terminal + Python + Git, código no computador.
**Fases 03–04:** Node/TypeScript, navegador devtools, banco local e API.
**Fases 05–06:** CI, Docker, deploy de teste, monitoramento e rollback.
**Fases 07–08:** APIs de IA por orçamento limitado, dados sintéticos, mecanismos de avaliação; alternativa com modelos simulados (*mocks*) sem gasto.
**Fase 09:** aplicações e demos públicas apenas sem segredos nem dados reais.

## Segurança inicial
Nunca enviar tokens, senhas, cookies de sessão, chaves de API, dados pessoais nem dumps de produção ao GitHub ou a agentes. Usar variáveis de ambiente, arquivos .env ignorados e contas de teste. Registrar custos, cotas e recursos criados. Em caso de vazamento, revogar segredo imediatamente.

## Quando o projeto começar a crescer
Criar `README` reproduzível, `.env.example` sem valores, `.gitignore`, dependências travadas, pipeline de testes e guia de rollback. Não introduzir ferramentas antes de justificar seu valor.
