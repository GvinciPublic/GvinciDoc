# Gvinci : Usando Map com parâmetros

O controle **Map** pode ter suas propriedades preenchidas através do uso de variáveis, parâmetros, alias ou campos, através do botão extensor de cada propriedade, utilizando a janela Fórmula.

![](http://www.gvinci.com.br/manual/formulanew.zoom78.png)

Neste tópico veremos como utilizar o **Map** através de parâmetros.

As propriedades do controle que podem ser preenchidas com valores de parâmetros são as seguintes.

![](http://www.gvinci.com.br/manual/propsmap.png)

Nossa aplicação exemplo terá somente duas páginas Aspx. Uma página \(Localização\) para exibir o controle **Map** com a localização do endereço solicitado e outra página \(Consulta\) para preencher controles **TextBox** com os valores que correspondem às propriedades citadas na figura acima, ou seja, os dados de endereço para a localização.

**1.** Em uma nova solução, insira dois módulos Página:

![](http://www.gvinci.com.br/manual/paginasmap2.png)

Nosso primeiro módulo terá o nome **"Consulta".**

**2.** Dê um clique duplo no primeiro módulo **"Página"** e preencha as propriedades conforme a figura abaixo. Lembre-se de desmarcar a opção **"Exigir autenticação"**, pois esta página não precisará de Login para ser exibida.

![](http://www.gvinci.com.br/manual/proppagmap.zoom92.png)

Nosso segundo módulo terá o título **"Localização"** e o nome **"PaginaMap"**.

**3.** Dê um duplo clique no segundo módulo **"Página"** e preencha com as propriedades conforme a figura abaixo. Novamente, lembre-se de desmarcar a opção **"Exigir autenticação"**.

![](http://www.gvinci.com.br/manual/localizamap.png)

Nosso próximo passo agora será inserir controles no Design das páginas criadas.

**4.** Selecione a página **"Consulta"** e clique em Design para inserirmos os controles.

![](http://www.gvinci.com.br/manual/designconsultamap.zoom88.png)

**5.** Insira um controle **Label** e na propriedade **Text,** coloque o seguinte texto: **"Consulta de endereços".**

**6.** Em seguida, insira mais 5 controles Label abaixo. Observe:

![](http://www.gvinci.com.br/manual/labelsmap.png)

**7.** Preencha a propriedade **Text de cada Label,** conforme os textos da figura abaixo:

![](http://www.gvinci.com.br/manual/labelsmap2.png)

**8.** Abaixo de cada Label, insira um controle **TextBox:**

![](http://www.gvinci.com.br/manual/textboxmap.png)

Vamos precisar agora preencher os apelidos \(Alias\) de cada TextBox que serão usados para enviar os valores aos parâmetros da Página Localização.

**9.** Preencha a propriedade Alias de cada **TextBox** com o valor ilustrado na figura abaixo:

![](http://www.gvinci.com.br/manual/textboxmap2.zoom83.png)

Agora vamos configurar a página Localização.

**10.** Abra o Design da página Localização e insira um controle **Map:**

![](http://www.gvinci.com.br/manual/map-pagina.zoom91.png)

As propriedades do controle Map que precisam ser preenchidas são as seguintes:

![](http://www.gvinci.com.br/manual/prop-map2.png)

Essas propriedades serão preenchidas através de parâmetros.

**11.** Com o Design da página **Localização** aberto, clique em **"Parâmetros";**

![](http://www.gvinci.com.br/manual/paramlocaliza.png)

12. Utilizando o botão ![](http://www.gvinci.com.br/manual/adicionar.png), insira 5 parâmetros com os nomes listados abaixo. Todos eles deverão possuir o **Tipo "Caracter".**

![](http://www.gvinci.com.br/manual/parammap1.png)

Com os parâmetros necessários já inseridos, vamos inserir um botão com evento de navegação para a página Consulta, de modo que possamos retornar à página Consulta após visualizarmos o endereço noMap.

**13.** No Design da página Localização, insira um controle Button na parte inferior da página. Na propriedade Text, coloque **"Nova consulta":**

![](http://www.gvinci.com.br/manual/botaonova.png)

**14.** Com o botão **"Nova consulta"** selecionado, clique no botão extensor do evento **OnClientClick;**

![](http://www.gvinci.com.br/manual/eventonovaconsulta.png)

**15.** Utilizando o botão ![](http://www.gvinci.com.br/manual/adicionar.png) para incluir uma ação de navegação, preencha as propriedades do evento conforme abaixo e clique em ![](http://www.gvinci.com.br/manual/ok-bt-2.jpg) :

![](http://www.gvinci.com.br/manual/naveganovaconsulta.png)

Agora voltaremos ao Design da página Consulta.

Precisaremos de um botão que irá exibir a página Localização e carregar os parâmetros. Este botão receberá um evento de navegação e irá enviar os valores dos "Alias" de cada controle para cada parâmetro correspondente da página Localização.

**16.** No Design da página **"Consulta"**, insira um controle Button no canto inferior da página. Na propriedade Text do botão, coloque o texto **"Consultar".**

![](http://www.gvinci.com.br/manual/buttonmap1.png)

**17.** Com o botão "Consultar" selecionado, clique no botão extensor do evento **OnClientClick:**

![](http://www.gvinci.com.br/manual/eventobotaomap.zoom86.png)

**18.** Utilizando o botão ![](http://www.gvinci.com.br/manual/adicionar.png), insira uma ação de Navegação e configure as outras propriedades do evento, conforme os dados na figura abaixo. Após preencher, clique em ![](http://www.gvinci.com.br/manual/ok-bt-2.jpg);

![](http://www.gvinci.com.br/manual/parameventos.zoom87.png)

Vamos agora definir os valores das propriedades do Map.

**19**. Selecione o controle **Map** na página Localização e, um de cada vez, clique no botão extensor das 5 propriedades na seção Location:

![](http://www.gvinci.com.br/manual/localizaalias.zoom74.png)

**20.** Na janela Fórmula, selecione o parâmetro correspondente e clique em ![](http://www.gvinci.com.br/manual/adicionar.png) , em seguida, clique em ![](http://www.gvinci.com.br/manual/okbt23.png). Repita este procedimento para preencher todas as 5 propriedades.

![](http://www.gvinci.com.br/manual/parammaps.zoom94.png)

Observe como deverão ficar as propriedades do **Map**, preenchidas:

![](http://www.gvinci.com.br/manual/propmapprontas.png)

Precisamos definir agora uma página inicial para a aplicação.

**21**. Clique com o botão direito em **"Consulta".** Selecione "Marcar como" e em seguida, clique em **"Página inicial";**

![](http://www.gvinci.com.br/manual/pginicialmap.png)

**22.** Salve a solução **&lt;Ctrl&gt; + &lt;S&gt;** e execute a geração de códigos **&lt;Ctrl&gt; + &lt;G&gt;.** Clique em Gerar.

![](http://www.gvinci.com.br/manual/gerarmap.png)

**23.** Clique em Abrir no Browser;

![](http://www.gvinci.com.br/manual/abrirbrowsermap.png)

A página principal, Consulta, será exibida no navegador padrão.

**24.** Preencha os dados corretamente e clique em Consultar.

![](http://www.gvinci.com.br/manual/pageconsulta.zoom91.png)

A página Localização será exida com o controle Map mostrando o endereço solicitado.

