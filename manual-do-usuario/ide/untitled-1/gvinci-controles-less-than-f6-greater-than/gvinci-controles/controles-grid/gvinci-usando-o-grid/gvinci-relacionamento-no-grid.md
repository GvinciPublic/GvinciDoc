# Relacionamento no Grid

O Controle Grid pode funcionar \(mas não necessariamente\) como um form filho, por exemplo, uma tabela vendas pode ser "pai" e a tabela **vendas\_itens** pode ser "filha". Nesse caso, um campo poderá ser escolhido para manter o relacionamento entre as duas, por exemplo, o campo **Código da venda.**

Para Inserir um relacionamento, utilize a propriedade **Relation.**

A tabela "pai" será a tabela básica da página de dados, no nosso exemplo aqui, a tabela **vendas.**

A tabela "filha" será a tabela que fornecerá os dados para o Grid, ou seja, a tabela **vendas\_itens.**

**1.** Após ter criado as tabelas com seus campos, insira um módulo **Página de dados** na árvore do projeto;

Alternativamente, você pode utilizar o botão "[Criar página de dados](http://www.gvinci.com.br/manual/criar_pagina_de_dados.htm)" no painel Banco de dados, após a definição da tabela, campos e índice.

**2.** Em seguida clique duas vezes sobre o módulo inserido para preencher suas propriedades:

![](http://www.gvinci.com.br/manual/definepgdadosgv5.png)

**3.** Clique sobre o botão ![](http://www.gvinci.com.br/manual/designbtgv5.png) para desenhar a tela.

**4.** Pressione simultaneamente **&lt;Ctrl&gt; + &lt;T&gt;** para formatar a tela, inserindo os controles que correspondem aos campos criados na estrutura da tabela básica da página de dados, exibida na figura acima.

**5.** Em seguida, insira um controle **Grid** na mesma página;

![](http://www.gvinci.com.br/manual/grid1gv5.zoom66.png)

Agora, vamos determinar qual será a tabela que vai fornecer os dados para o Grid.

**6.** Selecione o **Grid** e pressione **&lt;F4&gt;** para exibir o painel Propriedades;

**7.** Preencha a propriedade **Database** com o nome do banco de dados;

**8.** Preencha a propriedade **Table** com o nome da tabela que fornecerá os dados para o **Grid;**

**9.** Na propriedade **Relation,** clique no botão ![](http://www.gvinci.com.br/manual/extensor-botao.png) para construir um relacionamento entre a tabela "pai" e a tabela "filha". A tabela "Pai" será a tabela básica da página de dados, definida em suas propriedades no passo 1 acima. A tabela "filha" será a tabela que vai fornecer os dados para o Grid.

![](http://www.gvinci.com.br/manual/gridrelation411.png)

A janela de definição de relacionamento aparecerá. Observe a exibição dos campos das duas tabelas envolvidas: a tabela básica da página de dados do lado esquerdo e a tabela que vai fornecer os dados para o Grid do lado direito da janela.

![](http://www.gvinci.com.br/manual/relation2-0811.zoom83.png)

Observe que as duas tabelas contêm campos com índice: **"codvenda"** e **"coditemvenda"**. Estes campos serão usados para ligar as duas tabelas.

Devemos salientar, porém, que esses dois campos devem ser definidos como índices de suas respectivas tabelas.

![](http://www.gvinci.com.br/manual/relation-0811.zoom83.png)

**10.** Selecione o campo que será usado como ligação e clique em ![](http://www.gvinci.com.br/manual/adicionar.png). Desta forma, o quadro **"Expressão"** será preenchido com o relacionamento;

![](http://www.gvinci.com.br/manual/relationgrid25.zoom70.png)

**11.** Em seguida, clique em ![](http://www.gvinci.com.br/manual/ok2button.zoom72.png).

Pronto! O relacionamento foi definido.

