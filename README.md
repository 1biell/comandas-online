# Comandas Online — Sistema de Pedidos para Restaurantes

> Sistema web para gestão de pedidos em restaurantes, substituindo comandas em papel por um fluxo digital em tempo real entre garçom, cozinha e histórico.

![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
![Node](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-black?logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?logo=postgresql&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

---

## 📌 Sobre o Projeto

O **Comandas Online** digitaliza o processo de pedidos em restaurantes — do garçom à cozinha — eliminando erros de comunicação e perda de tempo com papel. Cada pedido é registrado, acompanhado em tempo real e arquivado no histórico.

---

## ✨ Funcionalidades

### 🧑‍🍳 Painel do Garçom
- Adicionar múltiplos itens em um único pedido
- Editar quantidade de cada item antes de enviar
- Enviar pedidos diretamente para a cozinha
- Visualizar pedidos mais recentes primeiro
- Paginação de pedidos (5 por página)

### 🍳 Painel da Cozinha
- Visualizar pedidos recebidos em tempo real
- Alterar status: **Pendente → Em Preparo → Concluído**
- Destaque visual por status com cores distintas
- Paginação de pedidos (5 por página)

### 📜 Histórico de Pedidos
- Consultar todos os pedidos concluídos
- Visualização de mesa, itens e horário
- Todos os horários no fuso horário America/Sao_Paulo
- Paginação (3 por página)

---

## 🛠️ Stack Tecnológica

| Camada | Tecnologias |
|--------|-------------|
| Frontend | React.js, HTML, CSS |
| Backend | Node.js, Express.js |
| Banco de Dados | PostgreSQL |
| Hospedagem do Banco | Render |

---

## 🚀 Como Rodar Localmente

### Pré-requisitos
- Node.js 18+
- PostgreSQL
- npm

### 1. Clone o repositório
```bash
git clone https://github.com/1biell/comandas-online.git
cd comandas-online
```

### 2. Configure o Backend
```bash
cd backend
npm install
```

Crie o arquivo `.env` com suas credenciais:
```env
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_HOST=host_do_banco
DB_NAME=nome_do_banco
DB_PORT=5432
```

Inicie o servidor:
```bash
node server.js
```

### 3. Configure o Frontend
```bash
cd ../Frontend
npm install
npm run dev
```

### 4. Acesse
- Frontend: http://localhost:5173
- Backend API: http://localhost:3000

---

## 📁 Estrutura do Projeto

```
comandas-online/
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── server.js
├── Frontend/
│   └── src/
├── .gitignore
└── README.md
```

---

## 🔒 Segurança

- Credenciais do banco protegidas via `.env`
- Arquivo `.env` ignorado pelo `.gitignore`

---

## 👨‍💻 Autor

Desenvolvido por **Gabriel Terra**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-gabrielnterra-0077B5?logo=linkedin&logoColor=white)](https://linkedin.com/in/gabrielnterra)
[![GitHub](https://img.shields.io/badge/GitHub-1biell-181717?logo=github&logoColor=white)](https://github.com/1biell)
