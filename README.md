# 🛒 MauiAppMinhasCompras - Gerenciamento de Compras com .NET MAUI e SQLite

Este projeto é uma aplicação mobile desenvolvida em **.NET MAUI** para o gerenciamento de compras pessoais. Nesta etapa do desenvolvimento, focamos na implementação da camada de persistência de dados utilizando o **SQLite**.

---

## 📌 Funcionalidades Desenvolvidas nesta Etapa

Nesta fase do projeto, foi implementada a classe auxiliar de banco de dados (`SQLiteDatabaseHelper`) responsável pelas operações CRUD na tabela de produtos:

- **Estruturação do Model:** Criação da classe `Produto.cs` com propriedades de `Id`, `Descricao`, `Quantidade` e `Preco`.
- **Conexão e Criação de Tabela:** Inicialização da conexão assíncrona com a base de dados SQLite (`SQLiteAsyncConnection`).
- **Inserção (`Insert`):** Método para cadastrar novos produtos.
- **Consulta Geral (`GetAll`):** Listagem de todos os produtos salvos no banco.
- **Busca por Descrição (`Search`):** Filtro de busca utilizando a instrução `LIKE`.
- **Atualização (`Update`):** Edição das informações de um produto existente.
- **Remoção (`Delete`):** Exclusão de registros com base no ID.

---

## 📹 Demonstração do Projeto (Vídeo)

Clique no link abaixo para assistir ao vídeo demonstrativo onde apresento a estrutura dos códigos criados e a execução do projeto no ambiente de desenvolvimento:

🔗 **[Assistir ao Vídeo de Demonstração no YouTube](https://youtu.be/ju7Yxt20B2I)**

---

## 🛠️ Tecnologias Utilizadas

- **C# / .NET MAUI** (Multi-platform App UI)
- **SQLite / sqlite-net-pcl** (Gerenciamento de Banco de Dados Local)
- **Visual Studio 2022**

---

## 📂 Estrutura das Pastas

MauiAppMinhasCompras/
│
├── Helpers/
│   └── SQLiteDatabaseHelper.cs   # Lógica do banco de dados SQLite (CRUD)
│
├── Models/
│   └── Produto.cs                # Classe de modelo do Produto
│
└── Views/
├── ListaProduto.xaml         # Interface da lista de produtos
└── NovoProduto.xaml          # Interface de cadastro de produtos
