# Gvinci : Inserindo um relatório Telerik

Neste tópico vamos inserir um relatório Telerik no exemplo Controle de Estoque.

O conteúdo deste tópico segue as instruções do vídeo listado ao final desta página.

**1.** Crie uma nova solução usando a aplicação exemplo Controle de Estoque, no menu Arquivo &gt; **Novo**;

![](http://www.gvinci.com.br/manual/arqnovoestgv5.zoom57.png)

**2.** Após criada a solução, abra o menu Módulos e arraste o módulo Relatório Telerik para a pasta Pages;

![](http://www.gvinci.com.br/manual/relattelerik1gv5.zoom62.png)

**3.** Dê um clique duplo sobre o nome do módulo Relatório - Telerik e preencha conforme a figura abaixo:

![](http://www.gvinci.com.br/manual/relattelerik2gv5.zoom74.png)

É necessário que o relatório tenha no mínimo uma fonte de dados para que os campos de uma determinada tabela possam ser utilizados.

**4.** Na seção **Fontes de dados**, clique no botão ![](http://www.gvinci.com.br/manual/adicion1gv5.png) para adicionar uma fonte de dados. Preencha com as sugestões abaixo e na lista de tabelas, selecione **TB\_PRODUTOS;**

![](http://www.gvinci.com.br/manual/relattelerik3gv5.zoom92.png)

**5.** Em seguida, clique no botão ![](http://www.gvinci.com.br/manual/telerikrepbt1gv5.png) para abrir a tela de relatório onde vamos inserir os campos que serão listados;

![](http://www.gvinci.com.br/manual/relattelerik4gv5.zoom90.png)

A tela do **Telerik Report Designer** será exibida conforme abaixo:

![](http://www.gvinci.com.br/manual/relattelerik5gv5.zoom62.png)

**6.** Clique na fonte de dados **GV\_DS\_Listaprodutos** para que sejam exibidos os campos da tabela na janela Data Explorer;

![](http://www.gvinci.com.br/manual/relattelerik6gv5.zoom63.png)

A figura abaixo apresenta descrições das 03 áreas do design do relatório:

![](http://www.gvinci.com.br/manual/relattelerik7gv5.zoom94.png)

A área HEADER \(cabeçalho\) pode ser usada para inserir os controles TextBox que serão usados como títulos de colunas e também pode ser usada para títulos do relatório, além de figuras usadas como logotipo de empresas.

Vamos inserir um título para o relatório.

**7.** Selecione a área **Header** do relatório e, com a aba **Insert** aberta, clique no controle **TextBox;**

![](http://www.gvinci.com.br/manual/relattelerik8gv5.zoom81.png)

**8.** Pressione **&lt;F2&gt;** e digite um título para o relatório. Redimensione o controle de modo a ficar semelhante à figura abaixo:

![](http://www.gvinci.com.br/manual/relattelerik9gv5.zoom88.png)

Agora vamos inserir uma figura para ser usada como logotipo da empresa.

**9.** Clique em PictureBox;

![](http://www.gvinci.com.br/manual/relattelerik10gv5.zoom82.png)

**10.** Arraste o controle para o canto esquerdo do HEADER:

![](http://www.gvinci.com.br/manual/relattelerik11gv5.zoom88.png)

**11.** Clique no botão ![](http://www.gvinci.com.br/manual/extensorbttgv5.png) da propriedade **Value;**

![](http://www.gvinci.com.br/manual/relattelerik12gv5.zoom67.png)

**12.** Localize a figura a ser inserida e clique em ![](http://www.gvinci.com.br/manual/abrirbtgv5.png);

![](http://www.gvinci.com.br/manual/relattelerik13gv5.zoom92.png)

Observe que a figura inserida ocupa toda a altura do Header:

![](http://www.gvinci.com.br/manual/relattelerik14gv5.zoom96.png)

**13.** Precisamos de espaço no Header para inserir os títulos de coluna. Por isso, vamos diminuir a altura da figura do logotipo, redimensionando o controle PictureBox. Outra solução seria aumentar a altura do Header.

![](http://www.gvinci.com.br/manual/relattelerik15gv5.zoom97.png)

**14.** Selecione a fonte de dados para visualizarmos os campos na seção Data Explorer. Neste relatório, vamo utilizar somente 03 campos: FD\_DESCRIÇÃO,  FD\_QTDE\_ESTOQUE e FD\_VALOR\_VENDA, em destaque na figura abaixo:

![](http://www.gvinci.com.br/manual/relattelerik16gv5.zoom73.png)

Por isso, vamos inserir somente 03 TextBox que serão usados como títulos das colunas no relatório.

**15.** Insira 03 controles TextBox na área HEADER e posicione conforme a figura abaixo:

![](http://www.gvinci.com.br/manual/relattelerik17gv5.zoom82.png)

**16.** Usando a tecla **&lt;F2&gt;,** digite os textos nos controles **TextBox** conforme as sugestões abaixo. Você pode usar os botões de ferramenta disponíveis em Text Box Tools para formatar o texto dos controles:

![](http://www.gvinci.com.br/manual/relattelerik18gv5.zoom77.png)

**17.** Clicando nos campos na seção **Data Explorer**, arraste-os e posicione logo abaixo dos títulos:

![](http://www.gvinci.com.br/manual/relattelerik19gv5.zoom61.png)

**18**. Clique no botão ![](http://www.gvinci.com.br/manual/salvarrelatbt1.png) para salvar o relatório.

![](http://www.gvinci.com.br/manual/relattelerik20gv5.zoom59.png)

Agora podemos fechar o relatório e gerar o código fonte.

Vídeo explicativo disponível pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[Relatório Telerik Gvinci Listagem de Produtos](https://www.youtube.com/watch?v=dPP5nx3Yu_k)

