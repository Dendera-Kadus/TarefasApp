# 📋 Sistema de Gestão de Tarefas

Este projeto é uma API REST desenvolvida em **.NET 8** utilizando os princípios de **DDD (Domain-Driven Design)** e arquitetura em camadas, com foco em boas práticas como Clean Architecture, separação de responsabilidades e automação de processos.

## 🎯 Objetivo

Permitir o cadastro, atualização, listagem e exclusão de tarefas. Cada tarefa possui título, descrição, status e responsável. Também é possível criar itens associados a tarefas, visando melhor organização do usuário. O sistema foi pensado para ser simples, mas organizado e fácil de manter.

## 🧱 Tecnologias Utilizadas

- ✅ [ASP.NET](http://asp.net/) Core Web API (.NET 6)
- ✅ Entity Framework Core
- ✅ SQL Server ou SQLite
- ✅ AutoMapper
- ✅ FluentValidation
- ✅ Swagger (Swashbuckle)
- ✅ Injeção de dependência nativa
- ✅ Clean Architecture + DDD

## 🗂️ Estrutura do Projeto

TarefasApp.sln

├── TarefasApp.API            // Camada de apresentação (controllers)

├── TarefasApp.Application    // Camada de aplicação (DTOs e serviços)

├── TarefasApp.Domain         // Domínio da aplicação (entidades, interfaces)

├── TarefasApp.Infrastructure // Acesso a dados (EF Core, repositórios)

## 🔄 Funcionalidades

- [ ]  Criar uma tarefa
- [ ]  Listar todas as tarefas
- [ ]  Atualizar o status de uma tarefa
- [ ]  Deletar uma tarefa
- [ ]  Filtros por status ou responsável *(em breve)*

## ▶️ Como rodar o projeto localmente

1. Clone o repositório
2. Abra a solução `TarefasApp.sln` no Visual Studio
3. Defina `TarefasApp.API` como projeto de inicialização
4. Configure a connection string no `appsettings.json`
5. Rode as migrations (opcional):
    
    Add-Migration InitialCreate
    Update-Database
    
6. Execute o projeto (F5 ou `dotnet run`)
7. Acesse a documentação Swagger:
    
    http://localhost:5000/swagger
    

## ✍️ Autor

Desenvolvido por **Dêndera Kadus Gomes**

🔗 [linkedin.com/in/dêndera-kadus](https://www.linkedin.com/in/d%C3%AAndera-kadus)

## 🚧 Em desenvolvimento...

Novas funcionalidades, testes unitários e melhorias de segurança serão adicionados futuramente.
