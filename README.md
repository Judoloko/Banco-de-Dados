# Banco-de-Dados
Atividade1: SQL Server 
O código apresentado é um conjunto de comandos DDL (Data Definition Language) em SQL Server para a criação de quatro tabelas em um banco de dados.
As tabelas são: Cliente, Apolice, Carro e Sinistro. Atividade realizada para FATEC Itapira, matéria de Banco de Dados, professor: Mateus Guilherme Fuini.

A tabela Cliente contém informações sobre os clientes da seguradora. 
Ela possui uma chave primária CodCliente, que identifica de forma única cada cliente. Além disso, a tabela possui outras colunas, como Nome, CPF, Sexo, Estado, Cidade, Bairro, Numero, Rua, TelefoneFixo e TelefoneCelular, que armazenam informações pessoais e de contato dos clientes. Algumas colunas possuem restrições, como a coluna Nome que não pode ser nula (NOT NULL), e as colunas CPF e TelefoneCelular que devem ser únicas (UNIQUE). A coluna Cidade possui um valor padrão definido como 'Itapira', ou seja, caso a informação não seja fornecida, esse será o valor padrão atribuído.

A tabela Apolice armazena informações sobre as apólices de seguro dos clientes. Cada apólice é identificada por um número único CodApolice. Além disso, a tabela possui outras colunas, como ValorCobertura, ValorFranquia, DataInicioVigencia, DataFimVigencia, Cliente_CodCliente e Carro_CodCarro, que armazenam informações sobre a cobertura do seguro, vigência da apólice, e quais carros e clientes estão associados a cada apólice. As colunas Cliente_CodCliente e Carro_CodCarro são chaves estrangeiras que se relacionam com a tabela Cliente e Carro, respectivamente.

A tabela Carro contém informações sobre os carros dos clientes da seguradora. Cada carro é identificado por um número único CodCarro. Além disso, a tabela possui outras colunas, como Placa, Marca, Modelo, Ano, Chassi e Cor, que armazenam informações sobre o carro de cada cliente.

Por fim, a tabela Sinistro armazena informações sobre os sinistros envolvendo os carros dos clientes. Cada sinistro é identificado por um número único CodSinistro. Além disso, a tabela possui outras colunas, como HoraSinistro, DataSinistro, LocalSinistro, Condutor e Carro_CodCarro, que armazenam informações sobre o horário, data, local, condutor e qual carro está envolvido em cada sinistro. A coluna Carro_CodCarro é uma chave estrangeira que se relaciona com a tabela Carro.
