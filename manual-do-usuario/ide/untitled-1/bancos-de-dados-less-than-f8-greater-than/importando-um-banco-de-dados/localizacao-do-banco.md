# Localização do banco

Para completar a importação do banco de dados, você deve preencher as seguintes opções, conforme mostra a figura abaixo:

![](http://www.gvinci.com.br/manual/localbdextgv5.zoom80.png)

**Servidor:** Neste campo você deve inserir o nome do servidor de banco de dados.

**Exemplo:** .\sqlexpress

O ponto \( . \) é usado para indicar o servidor local e "sqlexpress" é o nome da instância que foi definida na instalação do SQL Server.

**Autenticação:** A opção **Usar autenticação do windows \(Tusted Connection\)** pode ser usada quando:

• Nenhuma credencial é transmitida pela rede durante a autenticação, e você não precisa incorporar nomes e senhas de usuários na sequência de conexão do banco de dados. Isso significa que usuários mal-intencionados ou invasores não podem obter as credenciais por meio de monitoração da rede ou da exibição de sequências de conexão dentro de seus arquivos de configuração  
• Você obtém os benefícios do gerenciamento centralizado de contas. As contas de usuários estão sujeitas às diretivas normais de segurança do gerenciamento de contas, como períodos de vencimento e comprimentos mínimos de senhas e bloqueios de contas após várias solicitações inválidas de Logon

**Usar autenticação do Banco:** Ao marcar esta opção, será necessário inserir o nome do usuário e a senha que foram cadastrados na criação do banco.

**Banco de dados:** Permite escolher qual o banco de dados que será usado.

**Testar conexão:** Use este botão para testar a conexão antes de carregar o banco de dados. Caso a conexão seja efetivada, a mensagem abaixo é exibida:

![](http://www.gvinci.com.br/manual/conexaotestada.zoom100.png)

Após testar a conexão com sucesso, clique no botão ![](http://www.gvinci.com.br/manual/carregarbtgv55.png) para concluir o processo.

Toda a estrutura do banco importado poderá ser visualizada e alterada pelo **Gvinci.**

Caso você queira alterar a estrutura do banco importado e que essas alterações sejam também efetuadas no banco original, veja o tópico **Sincronizando bancos.**

