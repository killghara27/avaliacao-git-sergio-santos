# ECLIPSE: Guardiões das Trevas

**ECLIPSE: Guardiões das Trevas** é uma base de dados desenvolvida para representar a estrutura de um **videojogo online**, permitindo gerir jogadores, personagens, itens, quests e mascotes. O projeto foi desenvolvido em SQL com o objetivo de aplicar conceitos de bases de dados relacionais, como tabelas, chaves primárias, chaves estrangeiras e consultas SQL.

## 🎮 Funcionalidades

* Gestão de jogadores.
* Criação e gestão de personagens.
* Gestão de itens e inventário.
* Sistema de quests e recompensas.
* Gestão de mascotes.
* Diferentes classes de personagens, como Guerreiro, Xamã, Sura e Fada.
* Consultas SQL para pesquisa e análise dos dados.

## 🛠️ Tecnologias

|    Tecnologia   |  Versão  |
| :-------------: | :------: |
|      MySQL      |    8.0   |
| MySQL Workbench |    8.0   |
|       SQL       | Standard |
|      GitHub     |   Atual  |

### Estrutura da Base de Dados

A base de dados é constituída por várias tabelas relacionadas entre si:

* `jogador` — guarda a informação dos jogadores.
* `personagem` — guarda as personagens associadas aos jogadores.
* `item` — contém os itens disponíveis no jogo.
* `bolsinha` — relaciona os itens com as personagens.
* `quest` — contém as missões e respetivas recompensas.
* `guild` — contém as guilds.
* `mascote` — contém as mascotes.
* `loja` — contém os itens e mascotes que podem se adquiridos pelo personagem.

> **Nota importante:** As relações entre as tabelas são fundamentais para garantir a integridade e consistência dos dados.



## 💾 Instalação

Para utilizar o projeto localmente, é necessário ter o MySQL e o MySQL Workbench instalados.

1. Instalar o **MySQL**.
2. Instalar o **MySQL Workbench**.
3. Criar uma nova base de dados.
4. Executar o ficheiro `videojogoonline.sql`.
5. Confirmar que todas as tabelas foram criadas corretamente.
6. Executar as consultas SQL para testar a base de dados.

Exemplo de criação da base de dados:

```sql
CREATE DATABASE videojogoonline;

USE videojogoonline;

CREATE TABLE jogador ( 
    idjogador INT PRIMARY KEY AUTO_INCREMENT, 
    nome VARCHAR(100), 
    idade INT, 
    nacionalidade VARCHAR(100), 
    email VARCHAR(100) 
);

SELECT * FROM jogador;
```

O ficheiro principal do projeto é o `videojogoonline.sql`.

## 📋 Tarefas

### Estado do projeto

* [x] Criar a base de dados.
* [x] Criar as tabelas principais.
* [x] Definir chaves primárias.
* [x] Definir chaves estrangeiras.
* [x] Inserir dados de teste.
* [x] Criar consultas SQL.
* [ ] Adicionar novas quests.
* [ ] Adicionar mais itens e mascotes.
* [ ] Melhorar e expandir as consultas.



