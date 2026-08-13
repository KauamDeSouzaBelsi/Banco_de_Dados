##
Para apagar um banco de dados, utilizamos o comando

```sql
DROP DATABASE cidade;
```

> não esquecer do ;

---

**Modelagem do banco de dados**

```mermaid
erDiagram
PORDUTOS{
    int id PK "Gerado automaticamnete"
    varchar nome "Nome do produto"
    numeric valo "Preço do produto em R$"
    int estoque "Irá armazena a quantidade de produtos no estoque"
}
```

após modelar, iremos executar as etapas de criação e inserção de dados.
---
para criar a primeira tabela, usamos os comandos:
```sql
CREATE TABLE produtos(
    id INT GENERATED ALWAYS AS IDENTITY PRIMARY KEY, 
    nome VARCHAR(100) NOT NULL,
    valor NUMERIC(10,2) NOT NULL,
    estoque INT NOT NULL 0
);
```
---
Para consultar todos os itens da tabela, uso o comando
```sql
SELECT * FROM produtos;
```

---
para inserir dados na tabela, usamos:

```sql
INSERT INTO produtos(nome,valor,estoque)
VALUES('Caneta', '1.50','100');
```
---
**Crição do banco cidades**


![alt text](image-6.png)

>foi criado o banco cidades 
![alt text](image-7.png)

**No vscode**
>visão geral do codigo
![alt text](image.png)

>essa parte é a criação da tabela e oque vaui ter nela
![alt text](image-2.png)

>essa parte serve para pegar a tabela que acabamos de criar
![alt text](image-3.png)

>aqui é as informações que serão inseridas na tabela
![alt text](image-4.png)

>aqui é a tabela já com as informações
![alt text](image-5.png)