# TaskManager API 🗂️ ✅

Uma API REST simples feita em ASP.NET Core para gerenciar tarefas (como uma TODO list), criada como projeto de aprendizado ⚡

---

## 🛠️ Tecnologias Usadas

- ASP.NET Core 8
- C#
- Swagger (documentação da API)

---

## 🚀 Funcionalidades da API

| Método | Rota             | Descrição                        |
|--------|------------------|----------------------------------|
| GET    | /tasks           | Lista todas as tarefas           |
| POST   | /tasks           | Cria uma nova tarefa             |
| PUT    | /tasks/{id}      | Marca uma tarefa como concluída  |
| DELETE | /tasks/{id}      | Deleta uma tarefa específica     |

---

## 💻 Como rodar o projeto

### Pré-requisitos:
- [.NET SDK 8+](https://dotnet.microsoft.com/en-us/download)
- VS Code ou Visual Studio
- (Opcional) Postman ou REST Client (pode usar `TaskManager.http`)

### Passos:

```bash
# Clone o projeto
git clone https://github.com/seu-usuario/TaskManager.git

# Vá para a pasta do projeto
cd TaskManager

# Rode a aplicação
dotnet run
```
Abra no navegador:
🔗 https://localhost:5001/swagger — Documentação interativa com Swagger.

📁 Estrutura do Projeto
```bash
TaskManager/
├── Controllers/
│   └── TasksController.cs       # Define as rotas e lógica da API
├── Models/
│   └── TaskItem.cs              # Modelo de dados da tarefa
├── Properties/
│   └── launchSettings.json      # Configurações de ambiente
├── appsettings.json             # Configurações gerais
├── appsettings.Development.json # Configs para ambiente Dev
├── Program.cs                   # Entrada principal do app
├── TaskManager.csproj           # Arquivo de projeto .NET
├── TaskManager.http             # Arquivo de teste de requisições
```
🧠 Explicação das pastas
```bash
Controllers/ – Onde ficam os controladores da API (as rotas).
Models/ – Define os modelos de dados (como é uma "tarefa").
Program.cs – Inicializa e configura a aplicação.
Properties/ – Configurações do projeto.
appsettings.json – Semelhante a .env, armazena configs.
TaskManager.http – Permite testar as rotas direto no VS Code.
bin/ e obj/ – Pastas geradas automaticamente na build (podem ser ignoradas ou colocadas no .gitignore).
```

✨ Observações
Este projeto foi criado como exercício para aprender ASP.NET Core. Apesar de simples, cobre conceitos importantes como controllers, rotas REST, injeção de dependência (via builder.Services), estrutura MVC simplificada e uso do Swagger.
