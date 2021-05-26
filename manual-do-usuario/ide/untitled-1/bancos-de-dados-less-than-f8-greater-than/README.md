# Bancos de dados &lt;F8&gt;

O **Painel Bancos de Dados**, ilustrado abaixo, é exibido após clicar no botão ![](http://www.gvinci.com.br/manual/bferr9gv5.png).

Ao criar uma solução Default - na opção **Novo** do menu **Arquivo** - o **Gvinci** cria uma estrutura padrão para o primeiro banco de dados. Observe a figura abaixo mostrando as três tabelas que são criadas automaticamente quando se cria uma nova solução.

![](../../../../.gitbook/assets/image%20%2870%29.png)

### ![](http://www.gvinci.com.br/manual/adicion1gv5.png)**Incluir um novo Banco**

Permite adicionar um novo banco de dados.

### ![](http://www.gvinci.com.br/manual/excluibtgv5.png)**Exclusão do Banco**

Exclui o banco selecionado.

### ![](http://www.gvinci.com.br/manual/impxmlbdgv5.png)**Importar de um arquivo XML**

Importa estrutura do banco de dados de um arquivo XML. Este recurso pode importar, a estrutura de banco de dados criado pelos produtos GAS-2007/Father 1/Father 2/Father 3/ Father Next.

### ![](http://www.gvinci.com.br/manual/imp2bdgv5.png)**Importar de um banco de dados já existente**

Insere dados de um banco que já existe, após feita a conexão.

### ![](http://www.gvinci.com.br/manual/criarpgbtgv5.png)**Criar página de dados**

Permite gerar uma página de dados baseada na tabela selecionada.

### ![](http://www.gvinci.com.br/manual/criarrelatgv5.png)**Criar relatório**

Gera um relatório padrão baseado na tabela selecionada.

###   ![](../../../../.gitbook/assets/image%20%2869%29.png)**Gerar DDL \(DataBase Description Language\)**

Responsável por gerar o arquivos de script SQL para criação do banco de dados. Portanto, clicando nesse botão, apenas o script será atualizado sem necessidade de geração completa de códigos-fontes da solução.

{% hint style="info" %}
Indicado para uso em conjunto com o botão "Adaptar Banco", pois a adaptação do banco de dados é baseada no arquivo de script que o gera. Atualize o script e em seguida adapte o banco de dados.
{% endhint %}

### \*\*\*\*![](../../../../.gitbook/assets/image%20%2867%29.png) **Adaptar Banco**

Executa o aplicativo adaptador do banco de dados, que irá comparar a estrutura do banco de dados projetada com a estrutura real atualmente existente no banco de dados, conforme dados de conexão. Com esta operação, a estrutura definida no arquivo de script para criação do banco será usada para criação de um banco de dados temporário e comparação da nova estrutura com a estrutura existente. Com a existência de diferenças de estrutura, é fornecida interface para tomada de decisões que permitam adaptar a estrutura existente para a nova estrutura de modo que os dados armazenados possam ser devidamente aproveitados.

{% hint style="danger" %}
É sempre importante fazer backup do banco de dados antes de alterações estruturais.
{% endhint %}

Veja também "Adaptador de Banco de dados".

### ![](http://www.gvinci.com.br/manual/moveabaixobtgv5.png)Move o item selecionado para baixo.

### ![](http://www.gvinci.com.br/manual/moveacimabtgv5.png)Move o item selecionado para cima.

{% hint style="info" %}
Caso você prefira utilizar um banco já existente, veja o tópico [**Importando um banco de dados**](importando-um-banco-de-dados/)**.**
{% endhint %}

