# 🏎️ Formula 1 API

Uma API REST desenvolvida com **Fastify**, **TypeScript** e **Node.js** para disponibilizar informações sobre equipes e pilotos da Fórmula 1.

## 📋 Funcionalidades

* Listar todas as equipes
* Listar todos os pilotos
* Buscar um piloto pelo ID
* Suporte a CORS
* API construída com Fastify para alta performance

---

## 🚀 Tecnologias Utilizadas

* Node.js
* TypeScript
* Fastify
* Fastify CORS
* TSX
* TSUP

---

## 📁 Estrutura do Projeto

```bash
project-formula-1/
│
├── src/
│   └── server.ts
│
├── package.json
├── tsconfig.json
└── README.md
```

---

## ⚙️ Instalação

Clone o repositório:

```bash
git clone https://github.com/seu-usuario/project-formula-1.git
```

Entre na pasta do projeto:

```bash
cd project-formula-1
```

Instale as dependências:

```bash
npm install
```

---

## ▶️ Executando o Projeto

### Ambiente de Desenvolvimento

```bash
npm run start:dev
```

ou

```bash
npm run start:watch
```

A API ficará disponível em:

```text
http://localhost:3333
```

---

## 📌 Endpoints

### Listar Equipes

**GET**

```http
/teams
```

### Exemplo de Resposta

```json
{
  "teams": [
    {
      "id": 1,
      "name": "McLaren",
      "base": "Woking, United Kingdom"
    },
    {
      "id": 2,
      "name": "Mercedes",
      "base": "Brackley, United Kingdom"
    },
    {
      "id": 3,
      "name": "Red Bull Racing",
      "base": "Milton Keynes, United Kingdom"
    }
  ]
}
```

---

### Listar Pilotos

**GET**

```http
/drivers
```

### Exemplo de Resposta

```json
{
  "drivers": [
    {
      "id": 1,
      "name": "Max Verstappen",
      "team": "Red Bull Racing"
    },
    {
      "id": 2,
      "name": "Lewis Hamilton",
      "team": "Ferrari"
    },
    {
      "id": 3,
      "name": "Lando Norris",
      "team": "McLaren"
    }
  ]
}
```

---

### Buscar Piloto por ID

**GET**

```http
/drivers/:id
```

### Exemplo

```http
/drivers/1
```

### Resposta de Sucesso

```json
{
  "driver": {
    "id": 1,
    "name": "Max Verstappen",
    "team": "Red Bull Racing"
  }
}
```

### Resposta de Erro

```json
{
  "message": "Driver Not Found"
}
```

---

## 📦 Gerando Build

Para gerar os arquivos de produção:

```bash
npm run dist
```

Para executar a versão compilada:

```bash
npm run start:dist
```

---

## 🛠 Scripts Disponíveis

| Comando             | Descrição                        |
| ------------------- | -------------------------------- |
| npm run start:dev   | Executa a API em desenvolvimento |
| npm run start:watch | Executa com reload automático    |
| npm run dist        | Gera a build do projeto          |
| npm run start:dist  | Executa a versão compilada       |

---

## 📚 Objetivo do Projeto

Este projeto foi desenvolvido para praticar conceitos de:

* APIs REST
* Fastify
* TypeScript
* Rotas e parâmetros
* Tratamento de respostas HTTP
* Organização de projetos backend com Node.js

---

## 👨‍💻 Autor

Desenvolvido por **Giliarde Rodrigues** pelo curso da Dio.

Sinta-se à vontade para contribuir, abrir issues ou sugerir melhorias.
