# Aula 001 | Orientação do mentor (não ler antes da tentativa)

**O objetivo é raciocínio, não memorizar saídas.**

Casos críticos iniciais:
- `-1, 0, 300.01, "abc", null`: inválidos.
- `1, 59.99, 60`: uma porta.
- `60.01, 119.99, 120`: duas portas.
- `120.01, 299.99, 300`: três portas.

**Mudança >240:** obrigar revisão humana para largura estritamente maior que 240; `240` continua na faixa de 3 portas se contrato afirmar "acima de 240". Perguntar sobre o limite antes da implementação e cobrir `240`, `240.001`.

**Rubrica de correção:** entradas/saídas; exclusividade das faixas; checagem de inválidos antes das faixas; clareza do algoritmo; testes em limites; explicar diferença entre regra incompleta e código com bug; comunicação em inglês.

**Perguntas de aprofundamento**
- E se a medida estiver em mm?
- E se o sistema ler número como string? E " 60 "?
- E se o valor for `NaN` num ambiente específico?
- Em quem recai a responsabilidade por uma regra comercial insegura?
- Como dar feedback útil ao vendedor sem mostrar dados técnicos?

**Não marcar concluído até teste com casos não ensaiados.**
