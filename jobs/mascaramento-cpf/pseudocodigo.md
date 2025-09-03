## Pseudocódigo – Mascaramento de CPF

1. Para cada registro na tabela de origem:
   a. Verifica se o campo CPF está preenchido
   b. Se estiver vazio, atribui valor padrão "000.000.000-00"
   c. Se estiver preenchido:
      - Gera um número aleatório com 11 dígitos
      - Formata como CPF (###.###.###-##)
      - Atualiza o campo original com o novo valor
2. Garante que o CPF gerado não seja válido (evita colisão com CPFs reais)
3. Preserva integridade referencial se o CPF estiver relacionado a outras tabelas
