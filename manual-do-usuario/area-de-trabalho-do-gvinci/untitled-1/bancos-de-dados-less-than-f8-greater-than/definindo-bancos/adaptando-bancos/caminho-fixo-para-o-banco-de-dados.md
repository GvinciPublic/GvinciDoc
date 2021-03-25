# Caminho fixo para o banco de dados

Quando um projeto é gerado, o **Gvinci** cria um arquivo chamado **web.config** e o armazena dentro da pasta Projeto, que, junto à pasta Components, é criada no momento da geração do projeto. Para mais detalhes sobre como definir a pasta da solução, clique [aqui](http://www.gvinci.com.br/manual/local_da_solucao.htm).

O arquivo web.config é criado em formato XML e contém as configurações gerais para conexão Web.

Toda vez que a aplicação for gerada, será necessário confirmar a String de conexão para o banco de dados.

A string padrão é:

Server=.\gvinci;Database=Banco;User ID=sa;Password=gvinci;Trusted\_Connection=false

Esta String de conexão já vem inserida quando uma nova solução é criada. O usuário "sa" \(System Administrator\), a senha "gvinci" e o tipo de autenticação pelo banco "Trusted\_Connection=false" são configurações inseridas durante a instalação do SQL server, na instalação do Gvinci.

Ao desmarcar a opção "Editar string de conexão" no painel Banco de dados, o campo usado para edição "Connection String" é desativado e ao mesmo tempo, o botão "Configurar banco" é habilitado. Isso faz com que o caminho para o banco de dados seja armazenado no arquivo Web.config e não será mais necessário que o usuário indique a localização do banco.

![](http://www.gvinci.com.br/manual/bancofixgv5.zoom80.png)

Ao clicar no botão **"Configurar banco"**, a tela de configuração é aberta. O campo "Servidor" pode ser preenchido com o nome do servidor e a instância que já deverão ter sido definidos na instalação do SQL Server. Para detalhes, clique [aqui](http://www.gvinci.com.br/manual/configuracao_do_banco.htm).

A tela de configuração de banco de dados exibida abaixo mostra o campo Servidor preenchido com o servidor local \( . \) e a instância padrão "gvinci".

![](http://www.gvinci.com.br/manual/configbdtelagv5.zoom100.png)

Já definidos durante a instalação do SQL Server, foram configurados o usuário "sa" e a senha "gvinci".

A string padrão é:

Server=.\gvinci;Database=Banco;User ID=sa;Password=gvinci;Trusted\_Connection=false

**Server:** Indica o servidor de banco de dados. Na string acima, é o servidor local representado por um ponto \( . \).

**Database:** Define o nome do banco de dados que será criado ou aberto.

**Trusted Connection= False:** Indica o uso da "autenticação pelo banco".

Observe na string que a opção Trusted Connection está com o valor "false", ou seja, não usará autenticação do windows e sim a conexão do banco.

