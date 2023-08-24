## Desenvolvimento do Projeto
Este repositório contém o código e informações relacionadas ao projeto de integração de um banco de dados MySQL com o Power BI, desenvolvido como parte do curso da DIO (Digital Innovation One) no módulo 3.

### Etapas do Projeto
O desafio foi dividido em três etapas principais:

  1. Configuração da Infraestrutura
Criou-se uma conta na plataforma Azure (azure.com) para hospedar o banco de dados e outras soluções.

  3. Integração do Banco de Dados
Realizou-se a criação do banco de dados MySQL utilizando o MySQL Workbench.
Foi necessário criar um script SQL que definisse a estrutura das tabelas, incluindo conceitos de acesso e chaves estrangeiras.
Para inserção de dados, foi desabilitada temporariamente a verificação de chaves estrangeiras ("SET FOREIGN_KEY_CHECKS=0") para permitir a inserção adequada dos registros.
Após a inserção dos dados, a verificação de chaves estrangeiras foi reativada ("SET FOREIGN_KEY_CHECKS=1") para manter a integridade dos dados.

  4. Transformação e Visualização dos Dados
Realizou-se a transformação dos dados utilizando as funcionalidades de ETL/ELT do Power BI.
Foram realizadas análises para prática e entendimento dos conceitos aprendidos no curso da DIO (módulo 3).
A conexão com o banco de dados hospedado na Azure foi estabelecida para carregar a fonte de dados no Power BI.
Foi criado um script para uma nova fonte de dados utilizando o Direct Query, possibilitando uma conexão mais dinâmica e em tempo real.

## Artefatos de Entrega

**Os seguintes artefatos foram desenvolvidos como parte das entregas do projeto:**

- Tratamento de dados incompatíveis.
  
- Carregamento apenas das colunas das tabelas utilizadas.
  
- Conexão com o banco de dados hospedado na Azure.
  
- Script para nova fonte de dados utilizando Direct Query.
  
- Criação de análises para demonstrar o conhecimento adquirido.
  
- Pergunta sobre Mesclar e Atribuir (Item 14)
  
- No contexto supracitado, a função de "mesclar" se refere à aplicação de junções de tabelas, semelhante ao uso da cláusula JOIN em SQL. A função de "atribuir" - provavelmente se refere a operações de agregação, como soma ou contagem.

Por exemplo, ao mesclar duas tabelas usando uma chave comum, você combina os dados dessas tabelas em uma única tabela resultante, combinando linhas que possuem valores correspondentes na chave.

No entanto, a função de "atribuir" (agregar) é usada para resumir os dados. Por exemplo, você pode agrupar dados por uma coluna específica e, em seguida, calcular a soma ou a contagem de valores em outras colunas para cada grupo.

O motivo pelo qual você escolheria apenas a operação de mesclagem e não a de atribuição pode estar relacionado ao objetivo das análises. Se o foco for combinar informações de diferentes tabelas para análises mais detalhadas e comparativas, a mesclagem é mais apropriada. Se o objetivo for resumir e apresentar estatísticas sobre os dados, então as operações de agregação (atribuição) seriam mais relevantes.
