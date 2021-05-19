# Link na coluna do Grid

Ao utilizar um Grid, o **Gvinci** permite que você acesse uma página de outra tabela através de uma coluna específica.

Para inserir uma coluna que funcione como **link no Grid,** proceda da seguinte maneira:

**1.** Selecione a coluna do Grid que receberá o **link;**

**2.** Na propriedade **ColmunType,** selecione o valor **Hyperlink;**

![](http://www.gvinci.com.br/manual/hyperlinkgrd.zoom70.png)

Utilize a propriedade **LinkButtonText** para inserir um texto para o Link.

![](http://www.gvinci.com.br/manual/linkbttext.png)

**3.** Com a coluna selecionada, clique em Eventos, no painel Propriedades;

**4.** Clique no botão ![](http://www.gvinci.com.br/manual/extensor-botao.png) do evento **OnClick.** A janela de eventos aparecerá:

![](http://www.gvinci.com.br/manual/eventoslinkgv.png)

**5.** Clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png)  para adicionar um evento;

**6**. Na opção "Tipo da ação", selecione "Navegação";

![](http://www.gvinci.com.br/manual/eventosnavlink.png)

**7.** Na opção "Destino", insira o nome do módulo ao qual o Grid pertence;

**8.** Clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png) da opção "Navegar para:" e adicione o módulo para o qual o link servirá de acesso;

![](http://www.gvinci.com.br/manual/link-mod-gv.zoom74.png)

**9.** Clique em ![](http://www.gvinci.com.br/manual/okbt5.png).

Desta forma, o link está pronto para ser usado.

