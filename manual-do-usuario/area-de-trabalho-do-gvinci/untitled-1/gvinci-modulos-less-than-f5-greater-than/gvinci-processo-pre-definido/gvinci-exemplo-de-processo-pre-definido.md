# Gvinci : Exemplo de Processo Pré-definido

Neste exemplo, usaremos um processo pré-definido para reajustar preços de produtos. Vamos seguir as instruções abaixo:

**1.** Crie uma nova **solução;**

**2.** Clique duas vezes sobre "Título da solução" para exibir as propriedades;

**3.** Insira o nome da pasta onde será armazenada a solução;

![](http://www.gvinci.com.br/manual/propriedadesolucao911.zoom84.png)

**4.** Abra o painel **Banco de Dados** através do menu **Exibir**, para criarmos o banco de dados da aplicação;

![](http://www.gvinci.com.br/manual/bancodadosg.png)

Após abrirmos o painel Banco de dados, observamos que já existe um banco padrão **"Banco"** criado.Precisamos criar uma tabela para receber o cadastro dos produtos.

**5.** No painel **Banco de dados**, clique sobre a palavra **"Tabelas"** com o botão direito do mouse;

**6.** Clique sobre **"Nova tabela"**;

![](http://www.gvinci.com.br/manual/novatabela1411.png)

**7.** Altere as propriedades da nova tabela conforme figura abaixo:

![](http://www.gvinci.com.br/manual/bd1411.png)

Agora vamos criar dois campos básicos para a tabela **"Produtos"**.

**8.** Clique sobre **"Campos"** com o botão direito do mouse e em seguida, clique sobre **"Novo campo";**

![](http://www.gvinci.com.br/manual/novocampo1411.png)

**9.** Defina as propriedades do campo conforme abaixo:

![](http://www.gvinci.com.br/manual/definecampoproc411.png)

Agora vamos criar um campo onde poderemos cadastrar o valor do produto. Nosso campo terá o nome de **"Preço"**.

**10.** Clique sobre **"Campos"** com o botão direito e, em seguida, em **"Novo Campo"**;

**11.** Altere as propriedades conforme a figura abaixo:

![](http://www.gvinci.com.br/manual/definecampoproc2411.zoom101.png)

Agora precisamos criar um índice para a tabela Produtos.

**12.** Clique sobre **"Indices"** com o botão direito do mouse e em seguida, sobre **"Novo índice"**;

![](http://www.gvinci.com.br/manual/novoindiceproc411.png)

O **Gvinci** vai criar automaticamente um índice chamado **PK\_Produtos**, porém, é necessário determinar qual campo da tabela funcionará como índice. Vamos especificar isso no próximo passo:

**13.** Clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png) para adicionar um campo ao índice;

![](http://www.gvinci.com.br/manual/inserecampos411.png)

**14.** Clique duas vezes na opção de campo e selecione o campo **"Descprod"** para receber o índice;

![](http://www.gvinci.com.br/manual/inserecampos2411.png)

Agora que já temos a tabela Produtos criada, com dois campos e um índice, vamos criar uma página de dados que usará a tabela Produtos como tabela básica.

**15.** Com a tabela Produtos selecionada, clique no botão em destaque na figura abaixo para criar uma página de dados automaticamente;

![](http://www.gvinci.com.br/manual/criapagproc411.png)

Nosso próximo passo agora será criar uma página de processo pré-definido, que receberá o item de processo, mais tarde.

**16.** Com o painel Módulos aberto, clique sobre **"Processo pré-definido"** e arraste para o painel Módulos da solução, conforme figura abaixo:

![](http://www.gvinci.com.br/manual/insereprocesso911.zoom68.png)

**17.** Selecione o módulo **"Processo pré-definido"** e clique no botão ![](http://www.gvinci.com.br/manual/designbt411.png) para exibir o design, onde colocaremos os controles da tela do processo;

**18.** Com o painel Controles aberto, insira uma caixa de texto **\(TextBox\)** no design;

**19.** Insira o controle padrão **"Executa processo pré-definido"** no design;

![](http://www.gvinci.com.br/manual/executaprocesso411.zoom80.png)

Sua página de processo pré-definido deverá ter o seguinte layout:

![](http://www.gvinci.com.br/manual/designppd.png)

A caixa de texto exibida na figura acima é onde será inserida a porcentagem para fazer o cálculo sobre o conteúdo do campo **" preço"** da tabela Produtos. Durante a execução da aplicação, os campos e controles são chamados por seus apelidos \(Alias\). Por isso, precisamos adicionar um Alias para a caixa de texto da porcentagem.

**20.** Selecione a caixa de texto e pressione &lt;**F4**&gt; para exibir o painel Propriedades;

**21.** Insira a palavra **"Porcentagem"** na propriedade Alias da caixa de texto;

![](http://www.gvinci.com.br/manual/processopre411.zoom80.png)

Certifique-se de que a caixa de texto está habilitada para receber dados do tipo **"Number"**, que inclui números para a porcentagem.

**22.** Na propriedade **"Type"** da caixa de texto, coloque **"Number"**;

![](http://www.gvinci.com.br/manual/typenumber111.zoom73.png)

Mais adiante, quando formos inserir a fórmula do processo, o Alias da caixa de texto será usado.

**23.** Em seguida, com o painel Módulos aberto, insira um Item de processo no módulo Processo pré-definido;

![](http://www.gvinci.com.br/manual/itemproc.zoom73.png)

**24.** Para definir as propriedades do Item de processo, clique sobre **"Item de processo"** duas vezes;

![](http://www.gvinci.com.br/manual/propitemdeprocesso111.zoom87.png)

Neste exemplo, vamos utilizar o banco padrão - que possui o nome Banco - e a tabela **"Produtos"**.

**25.** Selecione o banco de dados que possui a tabela **"Produtos"**;

**26.** Na opção **"Tabela"**, selecione "Produtos".

Observe que a opção **"Provider"** será preenchida com o nome da tabela \(Produtos\). Quando a tabela **"Produtos"** foi criada no banco de dados, um provider com o mesmo nome também foi criado. Dois providers com o mesmo nome não podem ser usados, por isso, vamos alterar o nome do Provider na definição do processo pré-definido.

**27.** Insira um nome para o provider;

![](http://www.gvinci.com.br/manual/itemprocesso111.png)

Observe que os dois campos da tabela **"Produtos"** são exibidos na lista de campos que estão envolvidos no processo. Isso acontece porque a opção **"Utilizar todos os campos \(SELECT \*\)"** está marcada.

![](http://www.gvinci.com.br/manual/utilizacampos411.png)

Agora vamos configurar o item de processo.

**28.** Clique no botão **"Tabelas Auxiliares",** na parte inferior das propriedades;

![](http://www.gvinci.com.br/manual/itemprocesso2411.zoom94.png)

**29.** Em seguida, clique na aba **"Processos"**;

![](http://www.gvinci.com.br/manual/itemprocessos3411.zoom91.png)

Para o processo que vamos criar, definiremos um campo alvo, que receberá o processamento, e uma fórmula que determinará a forma que o processo será feito.

**30.** Crie um novo processo, clicando no botão ![](http://www.gvinci.com.br/manual/adicionar.png).

![](http://www.gvinci.com.br/manual/novoprocesso411.zoom73.png)

**31.** No campo Título, digite Reajuste;  


![](http://www.gvinci.com.br/manual/itemprocesso311.png)

**32.** Selecione o campo alvo para receber o processo. Neste caso, o campo **"Preco";**

![](http://www.gvinci.com.br/manual/itemprocesso41111.png)

**33.** Na opção **"Fórmula direta"**, clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png), para adicionar uma fórmula ao processo;

![](http://www.gvinci.com.br/manual/processonovo2411.zoom96.png)

A janela Fórmula será aberta. A expressão da fórmula será composta pelos nomes ou Alias \(apelidos\) dos campos e controles envolvidos no processo e os operadores que irão efetuar o cálculo. Observe na figura abaixo o Alias da caixa de texto **"Porcentagem"** em destaque.

![](http://www.gvinci.com.br/manual/processoformula5111.zoom74.png)

Agora, vamos construir nossa expressão para a fórmula que efetuará o processo. No exemplo que estamos utilizando, renomeamos o módulo de processo pré-definido para **"Reajustar preço"** e o item de processo para **"Reajuste".** Para detalhes, consulte o tópico "[Renomeando módulos](http://www.gvinci.com.br/manual/renomeando_modulos.htm)".

**34.** Utilize os botões ![](http://www.gvinci.com.br/manual/adicionar.png) e ![](http://www.gvinci.com.br/manual/menos.png) para adicionar e remover os campos no quadro Expressão. Clique nos botões dos operadores necessários para construir a expressão corretamente. A expressão pronta é exibida na figura abaixo:

![](http://www.gvinci.com.br/manual/formulaprocesso4111.zoom85.png)

Agora que o processo está completo, precisamos colocá-lo à disposição nas opções de menu.

A página Principal, criada automaticamente pelo **Gvinci**, apresenta uma barra de menus onde poderemos incluir os menus para cadastro de produtos e o menu que chamará a página do processo pré-definido.

**35.** No painel Módulos da solução, selecione com um duplo clique a Página principal;

![](http://www.gvinci.com.br/manual/ppdpgprincipal.png)

**36.** Selecione a barra de menus e pressione &lt;**F4**&gt; para exibir o painel Propriedades;

**37.** Clique no botão ![](http://www.gvinci.com.br/manual/extensor-botao.png) da propriedade Item da barra de menus para inserir os dois menus que precisamos;

![](http://www.gvinci.com.br/manual/ppdmenu.zoom71.png)

**38.** Insira um item de menu chamado **"Produtos"** e outro chamado **"Processo".** Em seguida, adicione os eventos de navegação para que esses menus chamem as páginas correspondentes. Para detalhes, consulte o tópico[Adicionando eventos a itens de menus](http://www.gvinci.com.br/manual/adicionando_eventos_a_itens_de.htm).

As páginas serão exibidas dentro do container **"IFrame"** e a barra de menus terá a seguinte aparência:

![](http://www.gvinci.com.br/manual/iframeppd.png)

**39.** Salve a solução e gere os códigos para executar a aplicação.

