# Gvinci : Adicionando eventos a itens de menus

Podemos utilizar um item de menu para abrir uma página ou para executar uma outra tarefa. Neste tópico veremos como adicionar um evento a um item de menu a fim de abrir uma página.

Uma barra de menus é geralmente apresentada em uma página principal que por sua vez deverá ter um controle **IFrame** para exibir outras páginas.

Para nosso exemplo, utilizaremos o módulo **Página** para construir uma página principal, conforme visto nos tópicos anteriores.

**1.** Primeiramente, insira uma barra de menu no design com três opções \(Para detalhes, consulte o tópico anterior\);

**2.** Altere a propriedade **Orientation** para **"Vertical";**

![](http://www.gvinci.com.br/manual/orientmngv5.zoom80.png)

**3.** Insira um controle **IFrame** para receber a página que será aberta;

![](http://www.gvinci.com.br/manual/ifrmmngv5.zoom80.png)

**4.** Selecione o menu desejado e, no painel **Propriedades,** clique no botão ![](http://www.gvinci.com.br/manual/eventosbt1gv5.png);

**5.** Clique no botão extensor ![](http://www.gvinci.com.br/manual/extensor-botao.png) do evento **Onclick;**

![](http://www.gvinci.com.br/manual/insevenmngv5.zoom80.png)

**6.** Em seguida, clique no botão ![](http://www.gvinci.com.br/manual/adicion1gv5.png) para adicionar uma ação;

![](http://www.gvinci.com.br/manual/addeventmngv5.zoom80.png)

**7.** Em **"Tipo da ação",** escolha **"Navegação";**

![](http://www.gvinci.com.br/manual/evnavmngv5.zoom80.png)

**8.** Na opção **"Destino"**, escolha o controle **IFrame1,** onde será inserida a página.

![](http://www.gvinci.com.br/manual/destevmngv5.zoom80.png)

**9.** Em **"Navegar para:"** clique no botão ![](http://www.gvinci.com.br/manual/adicion1gv5.png) para abrir a janela Módulos da solução;

![](http://www.gvinci.com.br/manual/evnnav2mngv5.zoom80.png)

**10.** Clique sobre a página desejada e em seguida no botão ![](http://www.gvinci.com.br/manual/btok1gv5.png);

![](http://www.gvinci.com.br/manual/pgprodmngv5.zoom80.png)

**11.** Na janela **Eventos**, clique em ![](http://www.gvinci.com.br/manual/btok1gv5.png).

Observe, no painel **Propriedades**, o evento que foi adicionado ao menu:

![](http://www.gvinci.com.br/manual/evnav3mngv5.zoom80.png)

