# Segurança, ética e responsabilidade técnica

Segurança e privacidade são parte da engenharia desde o primeiro dia, não um módulo decorativo no final.

## Obrigatório nos projetos
- Dados sintéticos e consentimento para qualquer dado não fictício.
- Princípio do menor privilégio; autenticação não é autorização.
- Validação do lado do servidor e tratamento explícito de erros.
- Segredos fora do repositório e fora dos prompts.
- Proteção a injeção SQL, XSS, CSRF e abuso de API, conforme contexto.
- Dependências verificadas, limites de taxa e logs sem conteúdo sensível.
- Backups, migrações, monitoramento e plano de recuperação quando aplicável.

## Segurança em aplicações com IA
- Documentos recuperados e respostas de ferramentas são **conteúdo não confiável**.
- Nunca executar ações externas irreversíveis sem regras, autorização e confirmação humana.
- Separar instruções de sistema, entrada do usuário e conhecimento recuperado.
- Escopar ferramentas; listas de permissões e validação de parâmetros.
- Avaliar vazamento de dados, alucinações, prompt injection e abuso.
- Registrar métricas e custos sem armazenar dados privados desnecessários.
- Não afirmar que RAG ou agentes são seguros só porque passaram nos testes felizes.

## Exercício transversal
Para cada grande entrega, criar um `THREAT_MODEL.md`: ativos, atores, fronteiras de confiança, principais abusos, mitigação e riscos remanescentes.

## Uso de IA no aprendizado
Não apresentar código de IA como autoria independente sem declarar assistência. Não copiar código, textos ou dados de terceiros sem verificar licenças e direitos.
