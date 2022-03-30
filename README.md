# CONTROLE DE ACESSO (Database) #
## Estrutura de tabelas para controle de acesso ##

Nesse script de banco de dados, são apresentadas tabelas e 
seus relacionamentos para serem utilizadas em um controle de acesso 
a funcionalidades de um sistema.


**Tabelas** e suas finalidades:

| Tabela                   | Finalidade                               |
|------------------------- | -----------------------------------------|
| login_usuario            | Relação de usuários                      |
| login_perfil             | Perfil de usuários (grupo de usuários)   |
| login_autorizacao        | Relação dos privilégios de acesso        |
| login_usuario_perfil     | Relação de usuários de um perfil         |
| login_perfil_autorizacao | Privilégios permitidos por perfil        |


**DER** - Diagrama-Entidade-Relacionamento
<img src='DER.JPG'>


## Ferramentas ##
Banco de dados [MySQL Server Community.](https://dev.mysql.com/downloads/mysql/5.6.html)

Gerenciador de banco de dados [MySQL Workbench.](https://dev.mysql.com/downloads/workbench/)


## Documentação ##
[MySQL Server 5.6.](https://dev.mysql.com/doc/refman/5.6/en/)

[MySQL Workbench.](https://dev.mysql.com/doc/workbench/en/)


## BCrypt ##
Para usar Hash BCrypt para encriptar a senha, deve-se alterar o tamanho da senha na tabela "login_usuario": senha varchar(62)

[Link para gerar senha.](https://bcrypt-generator.com/)

