  
Os comandos mais utilizados no MongoDB são aqueles que permitem realizar as operações básicas de um banco de dados, como criar, inserir, consultar, atualizar e excluir dados.

**Comandos para bancos de dados**

- **show dbs:** Lista todos os bancos de dados existentes.
- **use [nome_do_banco]:** Seleciona um banco de dados.
- **db.dropDatabase():** Exclui um banco de dados.

**Comandos para coleções**

- **show collections:** Lista todas as coleções existentes em um banco de dados.
- **db.createCollection([nome_da_coleção]):** Cria uma nova coleção.
- **db.collection.drop():** Exclui uma coleção.

**Comandos para documentos**

- **db.collection.insertOne([documento]):** Insere um novo documento em uma coleção.
- **db.collection.insertMany([documents]):** Insere vários documentos em uma coleção.
- **db.collection.find()::** Consulta todos os documentos em uma coleção.
- **db.collection.find({campo: valor}):** Consulta documentos que correspondem a um determinado critério.
- **db.collection.updateOne({campo: valor}, {novo_valor}):** Atualiza um documento existente.
- **db.collection.updateMany({campo: valor}, {novo_valor}):** Atualiza vários documentos.
- **db.collection.deleteOne({campo: valor}):** Exclui um documento existente.
- **db.collection.deleteMany({campo: valor}):** Exclui vários documentos.

**Outros comandos**

- **db.collection.renameCollection([nome_antigo], [nome_novo]):** Renomeia uma coleção.
- **db.collection.copyTo([nome_da_coleção]):** Copia uma coleção para outra.
- **db.collection.distinct([campo]):** Retorna um array com os valores únicos de um campo.
- **db.collection.count():** Conta o número de documentos em uma coleção.
- **db.collection.aggregate():** Aplica operações agregadas a uma coleção.

Esses comandos são suficientes para realizar a maioria das tarefas comuns em um banco de dados MongoDB. Para obter mais informações sobre cada comando, consulte a documentação oficial do MongoDB.

Aqui estão alguns exemplos de como esses comandos podem ser usados:

```
# Listar todos os bancos de dados
show dbs

# Selecionar o banco de dados "my_database"
use my_database

# Criar uma nova coleção chamada "customers"
db.createCollection("customers")

# Inserir um novo documento na coleção "customers"
db.customers.insertOne({name: "John Doe", age: 30})

# Consultar todos os documentos na coleção "customers"
db.customers.find()

# Consultar documentos que correspondem a um determinado critério
db.customers.find({age: 30})

# Atualizar um documento existente
db.customers.updateOne({name: "John Doe"}, {age: 31})

# Excluir um documento existente
db.customers.deleteOne({name: "John Doe"})
```