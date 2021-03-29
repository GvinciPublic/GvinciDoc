# Repeater com Filtro

Para inserir um filtro a um controle **Repeater**, podemos utilizar um **TextBox** para pesquisar os dados que desejamos. O valor da propriedade Alias deste **Textbox** será **"PesquisaValor"**.

Observe na página **"Lista de Clientes"** do exemplo **Burger Delivery Full**, o controle **txtPesquisa,** usado para a filtragem de dados:

![](http://www.gvinci.com.br/manual/repeaterfilter.zoom60.png)

Na página citada acima, o nome do cliente, telefone, bairro e endereço são exibidos na área chamada **Body do Repeater.**

Podemos utilizar o controle **txtPesquisa** para digitar o item que desejamos localizar e ele será então listado imediatamente no **Repeater,** após pressionar a tecla **&lt;Enter&gt;** ou clicar no botão ![](http://www.gvinci.com.br/manual/pesquisaicon.zoom69.png) .

Observe na figura abaixo, o item digitado no txtPesquisa é o único listado pelo Repeater:

![](http://www.gvinci.com.br/manual/repeaterfilter2.zoom79.png)

Para que o Repeater funcione conforme descrito, é necessário inserir um Filtro inicial na propriedade InitialFilter do Repeater:

![](http://www.gvinci.com.br/manual/repeaterfilter3.png)

A expressão de filtro que deve ser inserida é exibida na propriedade abaixo:

![](http://www.gvinci.com.br/manual/filtro-repeater.png)

O operador **"Like"** é utilizado, pois todo nome de cliente **\(\[CLI\_NOME\]\)** deverá ser igual ao digitado no **txtPesquisa**, que possui o alias **"PesquisaValor".**

Para configurar o botão que irá executar a pesquisa, o ícone ![](http://www.gvinci.com.br/manual/pesquisaicon.png), utilizamos um botão com a imagem padrão **"Magnfier"**.

![](http://www.gvinci.com.br/manual/magnifier.png)

Após inserir o botão com a imagem **Magnifier** na propriedade **BackgroundImage**, definimos um evento para o botão:

![](http://www.gvinci.com.br/manual/atualizarlist2.png)

Então, inserimos a função pré-definida **"Atualizar"** como ação do evento:

![](http://www.gvinci.com.br/manual/atualizarlistaclientes.png)

Desta forma, o controle **Repeater** terá seu filtro inicial executado sempre que o usuário clicar no botão para pesquisa ou pressionar a tecla Enter, após digitar os dados desejados no **Textbox** que possui o Alias "PesquisaValor".

![](http://www.gvinci.com.br/manual/aliastxtpes.png)

