## 🛡️ Boas práticas de LGPD e TDM (Test Data Management)

- Nunca use dados reais em ambientes de teste
- Sempre aplique técnicas de anonimização ou pseudonimização
- Documente o tipo de dado mascarado e a lógica aplicada
- Preserve integridade referencial entre tabelas
- Evite gerar dados válidos que possam coincidir com dados reais

Este guia é seu manual de referência para manter o repositório organizado, seguro e profissional. Se quiser, posso te ajudar a criar uma versão em inglês ou complementar com dicas de uso de branches e tags. Seu portfólio está com padrão de especialista! 💼📘

O Talend Open Studio for Data Integration, além de ser uma ferramenta de ETL, também realiza procedimentos de mascaramento de dados sensíveis e geração de dados sintéticos para testes nos procedimentos de Test data management – TDM​


O Mascaramento de Dados faz parte do Projeto LGPD e consiste em proteger dados pessoais nas bases de Desenvolvimento e Homologação;​

O processo atua alterando o conteúdo de campos que contém dados pessoais para dados fictícios .​

## Exemplos Funções​ ##

TalendDataGenerator.getFirstName() + " " + TalendDataGenerator.getLastName()  - mascarar nomes​

TalendDataGenerator.getUsStreet()   - bairro e endereço​

TalendDataGenerator.getUsStateId() -- estado​

TalendDataGenerator.getUsCity()  -- cidade​

Numeric.random(1,9999).toString()  - número de endereço

TalendDataGenerator.getUsStreet() + " - " + "numero" + " " + Numeric.random(111,999).toString() - complemento e endereço​

TalendDataGenerator.getFirstName()+ TalendDataGenerator.getLastName() + "@email.com"  - e-mail​

TalendDataGenerator.getFirstName()+ "mascaramento" + "@email.com"  - e-mail comercial​

UtilDev.getDDD() + " " + Numeric.random(111111111,999999999).toString() --telefone​

Numeric.random(111111111,999999999).toString() – cnh 9 dígitos
