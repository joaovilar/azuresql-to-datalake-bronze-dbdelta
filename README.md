# azuresql-to-datalake-medallion-dbdelta (in progress)
Este repositório contém scripts e pipelines para extrair dados de um banco de dados SQL Server (Azure SQL), transformá-los e carregá-los em um Data Lake no formato Delta.

![image](https://github.com/user-attachments/assets/20708519-b42a-4431-8a5a-17998a5a6699)


Utilizando o Delta Lake e o Databricks, o processo assegura a criação de tabelas bronze para armazenar dados brutos e realizar a ingestão contínua com controle de data e hora (timestamp), mantendo a integridade e a flexibilidade para futuras transformações.

Principais Funcionalidades:

    Conexão com Azure SQL Database usando JDBC.
    Extração de tabelas específicas do SQL Server para o Data Lake.
    Armazenamento de dados no formato Delta para garantir transações ACID.
    Adição de colunas de ingestão com timestamps para controle.
    Processamento de múltiplas tabelas de forma automatizada.

Tecnologias Utilizadas:

    Azure SQL Database
    Delta Lake
    Databricks
    Apache Spark
