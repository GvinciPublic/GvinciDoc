# Gvinci : Informações para Autenticação

As **informações para Autenticação** são necessárias para o controle de acesso de usuários. Esta opção oferece a possibilidade de cadastrar e remover usuários e grupos, bem como as regras correspondentes.

Observe abaixo os campos para autenticação, do exemplo Controle de Estoque.

![](http://www.gvinci.com.br/manual/infautentgv5.zoom80.png)

**Usuário Default:** Permite inserir um nome de usuário padrão para a tela de Login. O usuário padrão sugerido é **ADMIN.**

**Senha Default:** Permite inserir uma senha padrão para a tela de Login. A senha padrão sugerida é **ADMIN.**

Caso você tenha alterado a senha default e queira retornar para a senha ADMIN, é necessário apagar o registro de senha do usuário na tabela TB\_LOGIN\_USER, através do SQL Management Studio. Então, a senha ADMIN poderá ser definida novamente nas propriedades do projeto e poderá ser usada normalmente após a geração do código fonte.

**Banco de dados:** Insira o nome do banco que fornecerá os dados para o projeto.

**Criar estrutura default:** Permite criar uma estrutura padrão no banco de dados que poderá ser utilizada nas telas de Login em todos os projetos da solução. Esta estrutura já deverá conter as seguintes tabelas:

  
•Grupo de Login•Regras para Login•Usuário de Login

A figura abaixo mostra a estrutura padrão para informações de autenticação no banco de dados:

![](http://www.gvinci.com.br/manual/bdstructgv5.zoom80.png)

