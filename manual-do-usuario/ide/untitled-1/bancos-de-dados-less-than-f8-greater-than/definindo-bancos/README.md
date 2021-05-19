# Definindo bancos

Na parte superior direita do painel, escolhemos  as definições entre **L**ocal, **H**omologação e **P**rodução.

Ao selecionarmos o banco \(lado esquerdo do painel\) as deinifições são listadas no lado direto:

![Estrutura do banco de dados da aplica&#xE7;&#xE3;o exemplo Controle de Estoque](http://www.gvinci.com.br/manual/8_093.zoom80.png)

_Estrutura do banco de dados da aplicação exemplo Controle de Estoque_

![.](http://www.gvinci.com.br/manual/8_094.zoom80.png)

.

**Nome:** É o nome que será dado ao banco de dados no SQL. O Gvinci sugere o nome "Banco" a cada nova solução criada. Você deverá então definir um nome diferente. É importante que o nome do banco de dados não se repita, pois isso poderá causar dificuldades para conexão ao banco de dados.

**Apelido:** Insere um apelido\(Alias\) para o banco de dados. Este apelido será usado internamento pelo Gvinci.

**Título:** Insira o título do banco de dados.

**Principal:** Esta opção deverá ser marcada para somente um dos bancos de dados definidos, de modo a informar aoGvinci onde estarão as tabelas especiais para gerenciamento de senhas e controles de campos sequenciais que podem existir nas tabelas. O banco principal é sempre tratado com prioridade em operações de  pesquisa e filtragem.

**Tipo do banco :** Selecione o tipo de banco de dados a ser utilizado:

![](http://www.gvinci.com.br/manual/8_095.zoom80.png)

**Configuração de Delimitadores:** Alguns bancos de dados tem seus delimitadores específicos.

![](http://www.gvinci.com.br/manual/8_096.zoom80.png)

**Permitir adaptação:** Ao marcar esta opção, você permitirá que o banco seja adaptado quando houver alterações em sua estrutura.

**Nome do banco temporário:** Nome do banco utilizado para comparação de estrutura para adaptação de bancos.

**Verificar a existência do banco de dados:** serve para que quando for gerada a aplicação seja exigido a chamada da tela de configuração do banco de dados

**Editar string de conexão:** Ativa o campo **"Connection String"**, possibilitando a edição da string de conexão ao banco.

Ao desmarcar esta opção, o botão **"Configurar banco"** é ativado. Para detalhes veja o tópico **Caminho fixo para o banco de dados.**

Antes de especificar um caminho fixo para o banco de dados, é necessário que o banco já tenha sido criado.

**Connection String:** A string de conexão é a instrução que a aplicação vai utilizar para acessar o banco de dados, utilizando-se de um mecanismo - por exemplo, ADO.NET - que vai possibilitar a troca de informações entre a aplicação e o banco de dados através de um provider, que fornecerá essas informações.

**A String de conexão fornece dados como:** local\(servidor e instância\) e nome do banco, tipo de autenticação\(autenticação do Windows ou SQL\), usuário e senha \(quando for autenticação SQL\).

**A String de conexão padrão é:** Server=.\gvinci;Database=Banco;User ID=sa;Password=gvinci;Trusted\_Connection=false.

**Formato de data:** Define o formato que será usado para datas, de acordo com a configuração do servidor.

**Formato lógico:** Define o tipo de formato para Boolean \(Lógico - True ou False\).

**StartScripts:** Permite inserir scripts para serem executados na abertura do banco de dados.

**EndScripts:** Permite inserir scripts para serem executados no fechamento do banco de dados.

**Descrição:** Digite informações sobre o banco de dados em definição para que sejam utilizadas na documentação da aplicação, que é gerada pelo **Gvinci.**

Vídeo explicativo disponível pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[Diferentes configurações para bancos de dados, conforme o ambiente](https://www.youtube.com/watch?v=iE4ZlhoIA1Q)

