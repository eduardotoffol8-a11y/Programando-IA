# Fase 04 — Backend, HTTP e bancos de dados

**Semanas:** 27–34 · **Carga estimada:** 96 horas. Avance por domínio real, não automaticamente por data.

## Por que esta fase existe
Construir contratos de serviços seguros que preservem regras e dados entre requisições.

## Conhecimentos a dominar
cliente/servidor, TCP/IP/DNS básicos, HTTP status/methods, REST, JSON, OpenAPI, FastAPI, validação, migrations, SQL SELECT/JOIN/GROUP BY, tabelas/chaves, integridade referencial, normalização, índices, transações, autenticação vs autorização, pagination.

## Sprints semanais
| Semana | Tema | Entrega verificável |
|---|---|---|
| 27 | HTTP do começo ao fim | Rastrear clique até requisição/resposta, erros e cache. |
| 28 | SQL e modelagem | Criar esquema clientes/OS/itens com chaves e restrições. |
| 29 | Consultas e índices | Escrever JOIN, agregação e plano de consulta explicado. |
| 30 | FastAPI e contratos | Criar endpoints com validação e documentação de API. |
| 31 | Autenticação/autorização | Aplicar 2 papéis em rotas e consultas, cobrir negação. |
| 32 | Transações e idempotência | Proteger transição de estado e criar testes de repetição. |
| 33 | Integração frontend/backend | Erros previsíveis, paginação, conflitos e retry cuidadoso. |
| 34 | OficinaOS end-to-end | Demo com API/PostgreSQL e 20+ testes de integração. |

## Projeto de aplicação
OficinaOS funcional usando base sintética e permissão entre usuários.

## Gate obrigatório para prosseguir
Modelar e consultar banco, definir contrato, provar que usuário não acessa recurso alheio; defender decisão de índices.

## Inglês no trabalho
endpoint, payload, authorization, foreign key, migration, transaction, index, pagination.

## Referências
[PostgreSQL](https://www.postgresql.org/docs/current/tutorial.html) · [FastAPI](https://fastapi.tiangolo.com/tutorial/)

## Prova de autonomia
Resolver tarefa inédita sem IA (N0/N1), escrever casos-limite e registrar link de evidência, revisão e lição aprendida. Ver [rubrica](../AVALIACAO.md).

## Lição do mentor
Antes de mostrar sintaxe: perguntar o que é entrada, o que se transforma, que decisões existem, o que pode dar errado e como validar. Em seguida, exigir justificativa das escolhas técnicas.
