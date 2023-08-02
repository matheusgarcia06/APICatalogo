# API de Catálogos de Produtos

# Descrição 💻

Esta é uma API de catálogos de produtos que permite gerenciar categorias e seus respectivos produtos. A API foi desenvolvida utilizando .NET Core 6 e Entity Framework Core com abordagem Code First para a persistência de dados.

# Recursos 

A API fornece os seguintes recursos:

Gerenciamento de categorias: permite criar, recuperar, atualizar e excluir categorias.
Gerenciamento de produtos: permite criar, recuperar, atualizar e excluir produtos associados a uma categoria.

# Tecnologias Utilizadas

- .NET 6
- Entity Framework Core
- ASP.NET Core Web API
- Banco de Dados SQL Server

## Instalação e uso

```bash
# Abra um terminal e copie este repositório com o comando
git clone https://github.com/matheusgarcia06/APICatalogo
# ou use a opção de download.

# Navegue até o diretório do projeto.
cd APICatalogo

#Execute o aplicativo.
dotnet run

O aplicativo será executado em http://localhost:5000 (ou https://localhost:5001 com HTTPS ativado).
```

# Configuração do Banco de Dados
A API está configurada para utilizar o Entity Framework Core no modo Code First com um banco de dados SQL Server (ou outro banco de dados compatível). Para configurar o banco de dados, siga os seguintes passos:


```bash
# Abra o arquivo appsettings.json e altere a ConnectionString para apontar para o seu banco de dados SQL Server.
"ConnectionStrings": {
  "DefaultConnection": "Server=seu-servidor;Database=nome-do-banco;Trusted_Connection=True;"
}

# Execute as migrations para criar as tabelas do banco de dados.
dotnet ef database update
```

## Endpoints da API

# Categorias

GET /api/categorias: Retorna todas as categorias cadastradas.
GET /api/categorias/{id}: Retorna uma categoria específica pelo seu ID.
POST /api/categorias: Cria uma nova categoria.
PUT /api/categorias/{id}: Atualiza uma categoria existente pelo seu ID.
DELETE /api/categorias/{id}: Exclui uma categoria pelo seu ID.

# Produtos
GET /api/produtos: Retorna todos os produtos cadastrados.
GET /api/produtos/{id}: Retorna um produto específico pelo seu ID.
POST /api/produtos: Cria um novo produto associado a uma categoria.
PUT /api/produtos/{id}: Atualiza um produto existente pelo seu ID.
DELETE /api/produtos/{id}: Exclui um produto pelo seu ID.

# Autor

Matheus Garcia Nogueira

https://www.linkedin.com/in/matheusgarcianogueira/
