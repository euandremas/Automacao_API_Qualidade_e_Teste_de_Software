# 📦 Descrição do Repositório

**Automação de APIs – Qualidade e Teste de Software**

Repositório criado para a atividade final da disciplina **Qualidade e Teste de Software**, contendo a automação de testes de API utilizando **Postman** e **Newman**, com foco na validação de endpoints REST (status code, estrutura da resposta e tempo de resposta), conforme requisitos acadêmicos.

---

# 📘 README – Automação de Testes de API

## 🧪 Automação de Testes de API – DummyJSON

Este projeto foi desenvolvido como parte da **atividade final da disciplina Qualidade e Teste de Software (Unyleya)**, com o objetivo de aplicar na prática conceitos de **testes de API**, validações automatizadas e execução via linha de comando.

A automação utiliza a API pública **DummyJSON**, amplamente usada para estudos e práticas de QA.

---

## 🔧 Ferramentas Utilizadas

* **Postman** – Criação e execução dos testes de API
* **Newman** – Execução automatizada via terminal
* **DummyJSON API** – API pública para testes

---

## 🌐 API Testada

🔗 [https://dummyjson.com](https://dummyjson.com)

---

## 📂 Estrutura do Projeto

```
.
├─ collection/
│  └─ Automacao_API_DummyJSON.postman_collection.json
├─ README.md
```

---

## 🧠 Abordagem de Testes

Os testes de API foram organizados em coleções e pastas no Postman, cobrindo os seguintes cenários:

### 🔹 Autenticação (Auth)

* Login do usuário
* Validação de token

### 🔹 Produtos (Products)

* Adicionar produto
* Atualizar produto
* Remover produto

### 🔹 Usuários (Users)

* Adicionar usuário
* Atualizar usuário
* Remover usuário

---

## ✅ Validações Implementadas

Em todas as requisições foram aplicadas, no mínimo, as seguintes validações:

* Status code da resposta
* Estrutura do JSON retornado
* Tempo de resposta inferior a 2 segundos

---

## ▶️ Como Executar os Testes

### 1️⃣ Pré-requisitos

* Node.js instalado
* Postman instalado
* Newman instalado globalmente

```bash
npm install -g newman
```

---

### 2️⃣ Executar a automação via terminal

Na pasta onde está a collection:

```bash
newman run Automacao_API_DummyJSON.postman_collection.json
```

---

## 🎥 Evidências

* Execução dos testes via Postman
* Execução automatizada via Newman (terminal)
* Resultados exibidos no console

---

## 🎯 Objetivo Acadêmico

Este projeto consolida os seguintes aprendizados:

* Testes de API REST
* Automação de testes backend
* Validações automatizadas
* Uso de Postman e Newman
* Organização e documentação de testes

---

## 👨‍🎓 Autor

**André Santos**
Aluno de Análise e Desenvolvimento de Sistemas
Disciplina: Qualidade e Teste de Software

---
