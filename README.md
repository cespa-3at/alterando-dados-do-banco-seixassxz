[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/BipYyROc)
**Atividade: Atualização de Dados e Prova Real**

Nesta tarefa, você demonstrará domínio sobre o comando `UPDATE`. O desafio é alterar as informações de **todos os 3 contatos** que você criou anteriormente.

**Atenção:** Para esta tarefa, você deve **criar o banco de dados novamente** (ou editar o repositório antigo e realizar os novos prints no repositório atual). Os comandos de criação seguem a mesma lógica da atividade anterior.

**Objetivo**  
Atualizar registros específicos em uma tabela SQLite e validar as alterações com capturas de tela (prints) do "Antes" e do "Depois", utilizando obrigatoriamente o comando `SELECT`.

**Passo a Passo**

**1. Preparar o Banco de Dados**  
No terminal do seu Codespace, crie (ou abra) seu arquivo:

bash

```
sqlite3 seu_nome.db

```

_(Caso esteja criando do zero, lembre-se de rodar o `CREATE TABLE` e os 3 `INSERTs` iniciais antes de prosseguir)._

**2. Visualizar o Estado Atual (O "Antes")**  
Antes de qualquer mudança, mostre o que existe no banco atualmente.

- **Comando:** `SELECT * FROM contatos;`
- 📸 **PRINT 1:** Capture a tela mostrando os **3 registros originais**.

**3. Alterar os 3 Registros (UPDATE)**  
Você deve atualizar as informações (como telefone ou e-mail) de **cada um dos 3 contatos**. Use o `id` como referência para garantir a precisão:

- **Exemplo de comando (Repita para os IDs 1, 2 e 3):**

  sql

  ```
  UPDATE contatos SET telefone = 'Novo Telefone Aqui' WHERE id = 1;

  ```

**4. Validar as Alterações (O "Depois")**  
Após rodar os comandos de atualização para todos os registros, prove que os dados mudaram.

- **Comando:** `SELECT * FROM contatos;`
- 📸 **PRINT 2:** Capture a tela mostrando os **3 registros já alterados**.

**5. Sair e Salvar**  
Saia do SQLite digitando `.exit` ou `.quit`.

📤 **Entrega (Git & Documentação)**

Para a correção, você deve enviar o banco e as evidências:

1.  **Envie o arquivo .db para o repositório:**

    bash

    ```
    git add seu_nome.db
    git commit -m "Tarefa SQLite: Atualização completa dos 3 registros"
    git push origin main

    ```
