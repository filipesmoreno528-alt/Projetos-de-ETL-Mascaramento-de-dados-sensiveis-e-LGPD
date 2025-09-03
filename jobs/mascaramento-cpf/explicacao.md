## Explicação – Mascaramento de CPF

Este job realiza o mascaramento direto no campo original de CPF, utilizando funções randômicas para gerar novos valores com o mesmo formato. A técnica garante que os dados sejam anonimizados sem comprometer a estrutura da base, permitindo testes seguros em ambientes não produtivos.

O processo foi implementado no Talend Open Studio, com lógica de atualização (`UPDATE`) aplicada diretamente nas tabelas de destino. Os CPFs gerados são propositalmente inválidos para evitar qualquer risco de coincidência com dados reais.

Desafios enfrentados:
- Evitar duplicidade nos CPFs gerados
- Preservar integridade referencial entre tabelas
- Garantir performance em grandes volumes de dados

## 📸 Print do Job no Talend

![Fluxo Talend – CPF](screenshots/fluxo-cpf.png)


