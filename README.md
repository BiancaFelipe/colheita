# 🌱 API Colheita

<img width="1920" height="1080" alt="Green Illustrative Agriculture Presentation" src="https://github.com/user-attachments/assets/ab1beb7b-2178-49e6-87b4-2518b9643540" />

## Sobre a API

A **API Colheita** é uma aplicação voltada para **conectar produtores locais a consumidores**, promovendo a **economia local** e facilitando o acesso a **alimentos frescos e saudáveis**.  
O objetivo da API é permitir o **cadastro e gerenciamento de produtores e produtos**, fornecendo uma base para aplicações que valorizem o comércio local e a interação comunitária.

---

## Funcionalidades Principais

A API realiza operações **CRUD** (Create, Read, Update, Delete) para os seguintes recursos:

### Produtos
- **Create** – cadastrar novos produtos
- **Read** – listar produtos existentes
- **Update** – atualizar informações de produtos
- **Delete** – remover produtos

### Produtores
- **Create** – cadastrar novos produtores
- **Read** – listar produtores existentes
- **Update** – atualizar informações de produtores
- **Delete** – remover produtores

<p align="center">
  <img src="https://github.com/user-attachments/assets/7fc273d8-55b5-445f-8280-42ada5b436bc" alt="Gravação de tela">
</p>


---

## Executando o Projeto com Codespaces

Siga os passos abaixo para rodar a API utilizando o **GitHub Codespaces**:

1. Clique no botão **Code** (verde) no repositório.  
2. Selecione **Codespaces** → **New Codespace**.  
3. Quando o Codespace abrir, abra o **terminal**.  
4. Digite o comando para iniciar a aplicação:
```bash
npm run dev
```
5. Abra o navegador e acesse:
```bash
http://localhost:3000
```
6. Para visualizar os recursos da API:
- Para produtos: http://localhost:3000/api/products
- Para produtores: http://localhost:3000/api/producers

### Testando com POST
Para adicionar um novo produto via terminal:
```bash
curl -X POST http://localhost:3000/api/products \
-H "Content-Type: application/json" \
-d '{"name": "Tomate", "category": "Alimentos", "price": 5.50, "description":"Tomates Orgânicos da Fazenda do Sol", "quantity": 3, "producerId": 1}'
```

Para adicionar um novo produtor:
```bash
curl -X POST http://localhost:3000/api/producers \
-H "Content-Type: application/json" \
-d '{"name": "Fazenda do Sol", "location": "Cidade XYZ", "phone": "11923321909"}'
```

## Desenvolvedoras
- **Ana Catarina Mezzalira Romanosk Ribeiro** – Desenvolvimento principal da API
- **Bianca Felipe de Oliveira** – Contribuições adicionais e complementação do projeto.

## Contexto Acadêmico
Este projeto foi desenvolvido para o Projeto Integrador da disciplina Web Services, do professor Victor de Moura Indalécio.

## Licença
Projeto desenvolvido para fins acadêmicos e de aprendizado.
Pode ser estudado, adaptado e evoluído por outros estudantes, com os devidos créditos.
