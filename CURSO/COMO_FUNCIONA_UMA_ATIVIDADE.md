# Como funciona o laboratório de experiências profissionais

> Cada experiência é um ciclo realista de trabalho, mas em uma empresa **fictícia**. É prática supervisionada; não é emprego formal nem estágio.

## Toda atividade responde a oito perguntas

1. **Para quem trabalhamos?** Um cliente fictício, suas necessidades e quem será afetado.
2. **Qual problema estamos resolvendo?** O problema de negócio e sua consequência real.
3. **O que precisa ser entregue?** Arquivo, programa, funcionalidade ou correção observável.
4. **O que não podemos fazer?** Riscos, permissões, segurança, privacidade e escopo.
5. **Como saber se deu certo?** Testes, critérios de aceite e casos inesperados.
6. **Onde meu trabalho acontece?** No arquivo Markdown da primeira fase; depois em editores e ambientes de código.
7. **Como entrego?** Link do arquivo/commit; depois uma Pull Request com testes e documentação.
8. **Como sei se fui aprovado?** Revisão, desafio novo e registro de evidência no progresso.

## Seu dia típico na DEV FORGE Labs

| Etapa profissional | Tradução simples | Exemplo da Aula 001 |
|---|---|---|
| **Ticket / Issue** | Alguém entrega uma tarefa | “Definir quantidade inicial de portas” |
| **Requirements** | Descobrir regras e limites | “0 e acima de 300 são inválidos” |
| **Design** | Decidir como abordar | “Primeiro valido, depois comparo as faixas” |
| **Implementation** | Fazer a solução | Primeiro pseudocódigo humano; depois código |
| **Testing** | Tentar quebrar a solução | Entrada 60, 60.01, 120, 120.01, texto |
| **Code review / Review** | Outra pessoa questiona decisões | “Por que 120 tem duas portas?” |
| **Change request** | O cliente muda o pedido | “Acima de 240 precisa revisão humana” |
| **Demo / Handoff** | Mostrar e explicar a entrega | Explicação objetiva em português e inglês |

## Exemplo de uma situação concreta sem entregar a resposta

**Cliente fictício:** oficina de móveis sob medida.

**Problema:** orçamentos iniciais inconsistentes porque diferentes vendedores escolhem quantidades de portas diferentes para a mesma largura.

**Sua missão:** descrever um procedimento que uma máquina obedeceria, sem frases subjetivas, e detectar medições inválidas.

**Decisão real de engenharia:** ao receber exatamente 120 cm, o sistema deve aplicar a regra contratada, não “achar que o vão é grande”. Ao mudar o contrato para revisão humana acima de 240 cm, você deve ajustar o processo sem alterar os casos anteriores indevidamente.

**Evidência mínima:** uma tabela de entradas e saídas esperadas, regras claras, pseudocódigo, testes escolhidos por você e explicação de como trataria uma mudança.

**Pergunta de revisão:** “Se a saída estiver coerente com o programa, mas contrariar o contrato do cliente, o software está correto?”

## Como serão as experiências futuras?

### Experiência 1 — Analista de regras (Fase 00)
Interpreta a necessidade, modela dados, define limites e prevê falhas. Entrega Markdown, tabelas e pseudocódigo. Sem instalar nada.

### Experiência 2 — Desenvolvedor iniciante (Fases 01–02)
Implementa cálculos em Python, roda testes, entende mensagens de erro, usa Git e corrige bugs deliberadamente introduzidos.

### Experiência 3 — Time de produto (Fases 03–05)
Recebe tarefas de frontend, backend, banco de dados, API e autenticação; implementa em branches, abre PRs, trabalha com revisões e CI.

### Experiência 4 — Engenheiro de manutenção (Fase 06)
Recebe um sistema desconhecido com comportamento ruim; analisa logs, reproduz falhas, corrige com regressão e escreve postmortem.

### Experiência 5 — Engenharia de IA (Fases 07–08)
Cria assistente RAG, mede respostas corretas e incorretas; constrói agente com ações limitadas e aprovação humana para modificações sensíveis.

### Experiência 6 — Projeto de conclusão (Fase 09)
Recebe demandas, escreve especificação, implementa sistema completo, testa, apresenta e defende arquitetura em inglês.

## O mentor não deve trabalhar no seu lugar

Os níveis do curso:
- **N0:** você faz a tentativa sem IA.
- **N1:** IA só formula perguntas e dá pistas.
- **N2:** IA pode esclarecer conceitos e revisar depois de sua tentativa.
- **N3:** IA pode implementar partes, mas você responde pelas escolhas, segurança e testes.

**Regra de ouro:** abrir ou concluir uma issue prova organização; **domínio** só é registrado após demonstração e revisão. Ninguém deve prometer que um assistente humano/IA revisará automaticamente sem que haja de fato um encontro ou ferramenta acionada.

## Estrutura de um relatório de experiência

```text
Título:
Quem é o cliente (fictício ou autorizado):
Problema:
Restrições e riscos:
Entradas / saídas:
Plano inicial:
Testes que podem revelar erros:
O que produzi (link):
O que não funcionou:
Como corrigi:
O que a IA fez / o que eu fiz:
Explicação em inglês:
Feedback recebido:
Meu próximo passo:
```

## Siga em frente

- [Primeiro dia prático](PRIMEIRO_DIA.md)
- [Modelo real de resposta da Aula 001](templates/MODELO_ENTREGA_001.md)
- [Padrões de avaliação](AVALIACAO.md)
