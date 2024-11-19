# **Atividade: Implementação de um CRUD de Usuários**

## **Descrição da Atividade**
Seu objetivo é implementar um CRUD (Create, Read, Update, Delete) para gerenciar usuários em uma aplicação backend. Além de criar as rotas necessárias, você deve testá-las no Insomnia.

---

## **Requisitos**

### 1. **Estrutura do Usuário**
Cada usuário deve conter as seguintes informações:
- **ID:** gerado automaticamente.
- **Nome:** texto, obrigatório.
- **E-mail:** texto, único e obrigatório.
- **Senha:** texto, obrigatório (utilize hash para armazenamento, se possível).
- **Data de criação:** gerada automaticamente pelo sistema.

### 2. **Rotas do CRUD**
Implemente as seguintes rotas REST:

#### **Criar Usuário (POST)**
- **Rota:** `/users`
- Deve permitir a criação de um novo usuário com as informações necessárias.
- Valide os campos obrigatórios antes de salvar.

#### **Listar Usuários (GET)**
- **Rota:** `/users`
- Retorne uma lista de todos os usuários cadastrados.

#### **Obter Usuário por ID (GET)**
- **Rota:** `/users/:id`
- Retorne os dados do usuário com base no ID fornecido.

#### **Atualizar Usuário (PUT)**
- **Rota:** `/users/:id`
- Permita a atualização parcial ou completa dos dados de um usuário específico.

#### **Excluir Usuário (DELETE)**
- **Rota:** `/users/:id`
- Remova um usuário do sistema com base no ID fornecido.

### 3. **Testes no Insomnia**
- Crie uma coleção de requisições no Insomnia para testar todas as rotas.
- Certifique-se de que todas as requisições retornam os códigos de status HTTP apropriados:
  - **201** para criação bem-sucedida.
  - **200** para consultas ou atualizações bem-sucedidas.
  - **404** para usuário não encontrado.
  - **400** para erros de validação.
  - **500** para erros do servidor.

### 4. **Como subir as modificações pro Git**
Siga os passos abaixo para realizar o versionamento do seu trabalho:

**Crie uma branch para a atividade**  
   Use o comando abaixo para criar uma nova branch:
   ```bash
   git checkout -b Exercicio_seu_nome
```
**Adicione os arquivos ao stage
  Após realizar alterações no código, adicione os arquivos modificados para serem preparados para o commit:
```bash
  git add .
```
**Realize o commit
  Faça o commit com uma mensagem clara que descreva as alterações realizadas:
```bash
  git commit -m "sua mensagem do commit"
```
**Envie a branch para o repositório remoto
  Após finalizar suas alterações e realizar o commit, envie a branch para o repositório remoto:
  ```bash
  git push origin Exercicio_seu_nom
```
