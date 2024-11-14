
# Projeto de Autenticação com Envio de Email

Este é um projeto simples de autenticação em Node.js, que solicita ao usuário seu **email**, valida o input e envia um **email de confirmação** para o endereço inserido. Utiliza o **Nodemailer** para o envio de emails.

## Funcionalidades

- Exibe uma página de login solicitando o **email** do usuário.
- Após o envio do **email**, o servidor envia um **email de confirmação** para o endereço inserido.
- O **email de confirmação** contém uma mensagem simples informando ao usuário sobre o login.

## Tecnologias Usadas

- **Node.js** - Ambiente de execução JavaScript no servidor.
- **Express** - Framework web para Node.js.
- **Nodemailer** - Biblioteca para envio de emails.
- **Dotenv** - Gerenciamento de variáveis de ambiente (como as credenciais de email).

## Como Rodar o Projeto

### Passo 1: Clonar o Repositório

Clone este repositório para o seu computador:

```bash
git clone https://github.com/usuario/projeto-autenticacao.git
cd projeto-autenticacao
```

### Passo 2: Instalar Dependências

Instale as dependências do projeto com o comando:

```bash
npm install
```

### Passo 3: Configurar Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis:

```env
EMAIL=seuemail@gmail.com
PASSWORD=suaSenhaDeApp
```

> **Importante**: Para o envio de email com Gmail, é recomendado utilizar um **Token de App** em vez da senha normal da sua conta.

### Passo 4: Rodar o Servidor

Inicie o servidor com o comando:

```bash
npm start
```

O servidor ficará disponível em `http://localhost:3000/`.

### Passo 5: Acessar o Formulário de Login

Abra o navegador e acesse `http://localhost:3000/` para preencher o **email**. Após o envio do formulário, um email de confirmação será enviado ao endereço informado.

## Estrutura de Pastas

```
.
├── server
│   ├── controllers
│   │   └── authController.js  # Lógica de autenticação e envio de emails
│   ├── routes
│   │   └── authRoutes.js      # Definição das rotas
│   ├── server.js              # Arquivo principal do servidor
├── public
│   ├── login.html             # Página de login (entrada do email)
├── .env                       # Variáveis de ambiente para credenciais de email
├── package.json               # Dependências e scripts do projeto
└── README.md                  # Este arquivo
```

## Licença

Este projeto está licenciado sob a **MIT License**.

---

Esse **README** fornece uma explicação concisa do projeto, como rodá-lo, configurar as variáveis de ambiente e o que esperar do funcionamento.
