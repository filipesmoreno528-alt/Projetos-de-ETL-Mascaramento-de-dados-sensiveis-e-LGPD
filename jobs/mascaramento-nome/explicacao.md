## Explicação – Mascaramento de Nome

Este job substitui nomes reais por nomes fictícios, utilizando uma lista randômica previamente definida. O objetivo é garantir anonimização sem perder a estrutura dos dados, permitindo testes com campos realistas.

O processo foi implementado no Talend com lógica de atualização (`UPDATE`) e integração ao fluxo de ETL. A estrutura nome + sobrenome foi mantida para preservar a consistência dos dados.


## Explicação – Mascaramento de Endereço

Este job substitui endereços reais por dados fictícios gerados de forma randômica, mantendo o formato padrão (rua, número, bairro). A técnica garante anonimização dos dados sensíveis e viabiliza testes em ambientes seguros.

A lógica foi implementada no Talend com funções randômicas e listas de apoio. O campo original é atualizado diretamente, respeitando a estrutura esperada pelos sistemas consumidores.





## 📸 Print do Job no Talend

![Print do Job](screenshots/Job_mascaramento_estrutura.png)

