## Pseudocódigo – Mascaramento de Nome

1. Para cada registro na tabela:
   a. Verifica se o campo Nome está preenchido
   b. Se estiver vazio, atribui "Nome Genérico"
   c. Se estiver preenchido:
      - Gera um nome aleatório a partir de uma lista fictícia
      - Mantém estrutura de nome + sobrenome
      - Atualiza o campo original com o novo valor



## Explicação – Mascaramento de Endereço

Este job substitui endereços reais por dados fictícios gerados de forma randômica, mantendo o formato padrão (rua, número, bairro). A técnica garante anonimização dos dados sensíveis e viabiliza testes em ambientes seguros.

A lógica foi implementada no Talend com funções randômicas e listas de apoio. O campo original é atualizado diretamente, respeitando a estrutura esperada pelos sistemas consumidores.

**Desafios enfrentados:**
- Evitar colisão com endereços reais
- Preservar formato e consistência entre campos relacionados (CEP, cidade)
- Garantir performance em grandes volumes
