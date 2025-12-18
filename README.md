# 📘 README – Automação de Testes de API

## 🧪 Automação de Testes de API – DummyJSON

Este projeto foi desenvolvido como parte da **atividade final da disciplina _Qualidade e Teste de Software_ (Unyleya)**, com o objetivo de aplicar na prática conceitos de **testes de API**, **validações automatizadas** e **execução via linha de comando**.

A automação utiliza a **API pública DummyJSON**, amplamente empregada para estudos e práticas de **QA e automação backend**.

---

## 🔧 Ferramentas Utilizadas

- **Postman** – Criação, organização e execução dos testes de API  
- **Newman** – Execução automatizada das collections via terminal  
- **Node.js** – Ambiente para execução do Newman  
- **DummyJSON API** – API pública utilizada nos testes  

---

## 🌐 API Testada

🔗 https://dummyjson.com  

---

## 📂 Estrutura do Projeto

.
├─ Atividade_Final_API.postman_collection.json
├─ README.md
└─ newman-report.html (gerado na execução via Newman)


---

## 🧠 Abordagem de Testes

Os testes de API foram organizados em **uma collection no Postman**, cobrindo cenários funcionais e de autenticação, conforme descrito abaixo.

### 🔐 Autenticação (Auth)

- Login do usuário (`/auth/login`)
- Captura automática do **accessToken**
- Armazenamento do token, userId e username como variáveis da collection
- Validação de autenticação do usuário (`/auth/me`)
- Verificação se o token pertence ao usuário correto

---

### 📦 Produtos

- Adicionar produto
- Atualizar produto
- Remover produto

---

### 👤 Usuários

- Adicionar usuário
- Atualizar usuário
- Remover usuário

---

## ✅ Validações Implementadas

Em todas as requisições foram aplicadas, no mínimo, as seguintes validações automatizadas:

- ✔️ Código de status HTTP correto  
- ✔️ Tempo de resposta inferior a **2 segundos**  
- ✔️ Estrutura do JSON retornado  
- ✔️ Existência de campos obrigatórios  
- ✔️ Validação de autenticação via **Bearer Token (JWT)**  

---

## 🔐 Autenticação via Token

- O token JWT é capturado no login
- O token é armazenado como variável da collection
- A collection utiliza **Bearer Token dinâmico**
- O endpoint `/auth/me` valida se o token pertence ao usuário autenticado

---

## ▶️ Como Executar os Testes

### 1️⃣ Pré-requisitos

- Node.js instalado  
- Postman instalado  
- Newman instalado globalmente  

2️⃣ Executar a automação via terminal

Na pasta onde está o arquivo da collection:

newman run Atividade_Final_API.postman_collection.json

📊 Execução com Relatório HTML (Opcional)

newman run Atividade_Final_API.postman_collection.json -r cli,htmlextra --reporter-htmlextra-export newman-report.html

O relatório será gerado em formato HTML, contendo o detalhamento da execução.

🎥 Evidências

Execução dos testes via Postman

Execução automatizada via Newman (terminal)

Resultados exibidos no console

Relatório HTML gerado pelo Newman

🎯 Objetivo Acadêmico

Este projeto consolida os seguintes aprendizados:

Testes de API REST

Automação de testes backend

Validações automatizadas

Uso de Postman e Newman

Autenticação via JWT

Organização e documentação de testes

👨‍🎓 Autor

André Santos

Aluno de Análise e Desenvolvimento de Sistemas

Disciplina: Qualidade e Teste de Software

Instituição: Unyleya


