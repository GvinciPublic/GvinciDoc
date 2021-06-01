# Módulo: Página

![](../../../../../.gitbook/assets/image%20%2878%29.png)

### Título

Campo obrigatório que define o título da página que irá aparecer tanto na árvore do projeto quanto na barra de título do navegador na aplicação final.

O ícone do globinho ao lado direito do campo, ao ser clicado, pode definir o texto para cada idioma cadastrado na solução. \(Ver [idiomas da solução](../../../../trabalhando-com-a-solucao/definindo-solucao.md)\)

### Nome

Campo obrigatório que define o nome do arquivo .aspx gerado na pasta do projeto. O nome precisa ser único. Caso defina um mesmo nome de arquivo já existente, independente de estar ou não em outra pasta, o campo será contornado de vermelho com o alerta de que já existe arquivo com mesmo nome.

### Rota

Define um caminho de rota para navegação para a página. O nome da rota será usado como identificação para navegação, independente do nome físico do arquivo .aspx. Assim, se uma página estiver dentro de várias subpastas e o nome de rota para ela seja "Vendas", ao usar o nome do domínio seguido da rota "Vendas", a navegação ocorrerá para a página .aspx correspondente. Exemplo:

Caminho completo:

http://www.meudominio.com.br/Vendas/Comercial/Interno/Vendas.aspx

Caminho acessado por rota:

http://www.meudominio.com.br/Vendas

As rotas também podem receber parâmetros como segmentos da URL \(caminho\). Assim, se definir na aba de "Parâmetros" alguns parâmetros, estes poderão ser adicionados ao nome da rota, separados por / \(barra\) e entre { } \(chaves\). Exemplo:

http://www.meudominio.com.br/Vendas/{ParCodigoVenda}

Poderá usar vários segmentos na composição da rota, acrescentando os parâmetros necessários.

Dessa forma, nos eventos de navegação que apontem para a página com a rota, os parâmetros definidos poderão ser recebidos pela página. Vale lembrar que para esse caso, os parâmetros usados deverão ser fornecido valor, obrigatoriamente.

Abaixo, exemplo de definição de parâmetros para uma página:

![](../../../../../.gitbook/assets/image%20%2864%29.png)

Definição de Rota que permite o recebimento de parâmetros por meio de eventos de navegação:

![Rota Vendas e 2 segmentos trazendo nomes de par&#xE2;metros entre chaves.](../../../../../.gitbook/assets/image%20%2859%29.png)

{% hint style="info" %}
Sempre que for usar parâmetros que possam ser opcionais, defina-os no final da lista de parâmetros na definição de Rota. Assim eles poderão ficar sem receber valor e sem provocar erro por falta desses valores.
{% endhint %}

{% hint style="success" %}
Ao usar rotas, o caminho físico dos arquivos não é exposto, aumentando o nível de segurança da sua aplicação. Use em conjunto com a definição "Permitir acesso direto pela URL".
{% endhint %}

Ver [Trabalhando com Rotas](../../../../untitled-2/rotas.md)

### Somente design

Com essa opção selecionada, a aba "Design" fica disponível para desenho da interface, podendo arrastar e soltar controles na tela. Nesse modo, as abas C\# e JavaScript complementam a página Aspx com codificação para o code-behind do lado servidor e cliente, respectivamente.

Ver [Design](../../design/)

### Somente código

Com essa opção selecionada não ficará disponível a aba "Design", mas tão somente as abas de edição de código C\# e Aspx. Assim, tanto poderá editar completamente a página aspx com a codificação de páginas ASP.NET.

Dessa forma, todo o código inserido na aba Aspx será de sua inteira responsabilidade, não ocorrendo nenhuma modificação realizada pelo Gvinci de modo que não interfira em qualquer customização que realize.

{% hint style="warning" %}
Observe que nesse modo a aba JavaScript não é habilitada. Podendo acrescentar o código javascript através da tag apropriada para isso &lt;script&gt;. Ou seja, o controle total da codificação realmente fica a cargo do desenvolvedor.
{% endhint %}

{% hint style="danger" %}
O Gvinci não faz nenhum controle de possíveis erros inseridos nessa codificação manual.
{% endhint %}

### Exigir autenticação

Ao marcar essa opção, a página só poderá ser carregada após ocorrer autenticação por meio de um login. Sendo requisitada a página e não tendo ainda sido feita a autenticação ou o tempo de autenticação \([Session Timeout](../../../../trabalhando-com-a-solucao/definindo-projeto/)\) tenha esgotado, a [página padrão de login](../../../../trabalhando-com-a-solucao/definindo-projeto/) será invocada para em seguida exibir a página requisitada.

### Mobile

Acrescenta um ViewPort à página, permitindo um melhor ajuste de dimensões do conteúdo para dispositivos mobile como smartphones ou tablets que possuem telas menores.

Dessa forma, o conteúdo de páginas web, originalmente pensadas apenas para computadores, com design fixo e tamanhos mais largos, tem sua escala reduzida para que encaixem melhor na área visível de dispositivos móveis.

Abaixo é apresentada meta tag que é acrescentada ao código de páginas que estão com a opção "Mobile" marcada a fim de obter o ajuste necessário. São, pois, instruções passadas ao navegador a fim de instrui-lo de como controlar dimensões e escala das páginas.

```text
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=0" />
```

Veja também: [The ViewPort](https://www.w3schools.com/css/css_rwd_viewport.asp).

{% hint style="success" %}
Não se preocupe que isso é feito de forma automática pelo Gvinci, não precisará interferir na codificação desse recurso.
{% endhint %}

### Permitir acesso direto pela URL

Para acesso a determinada página na internet, utilizamos sua URL, que é o localizador do recurso demandando ou clicamos em algum link de alguma página já aberta. Nos browsers \(navegadores\) a barra de endereços é usada para se especificar o caminho da página a ser carregada e por meio dessa propriedade podemos restringir o acesso direto. Assim, se o caminho for digitado na barra de endereços do navegador o recurso não será permitido. Sendo viável apenas a abertura da página por meio de ações de botões, links ou outras interações que forem definidas em projeto.

No exemplo abaixo, a página especificada na barra de endereços, só poderá ser acessada diretamente, caso tenha permissão para isso. Caso contrário, somente acessará a página desejada, caso haja algum link que leve diretamente a ela, mas não pela barra de endereços.

![](../../../../../.gitbook/assets/image%20%2853%29.png)

### Layout Responsivo

Habilita uso de controles responsivos, acrescentando ao código da página a referência necessária para carga do [Bootstrap](../../../../../leituras-complementares/bootstrap.md) na aplicação final, conforme exemplo abaixo:

```text
<link rel="stylesheet" href="<%= ResolveUrl("~/Styles/bootstrap.min.css??sv=1.0_20210520182241") %>" type="text/css" media="screen" title="no title"/>
```

Ao se marcar a opção Layout Responsivo, também a opção Mobile é marcada automaticamente. Assim como, também é criado um ViewPort para apresentação corretas das páginas em dispositivos móveis.

{% hint style="info" %}
Com a opção marcada, estarão disponíveis em módulo do tipo Página os controles Carousel, LayoutCol, LayoutContainer, LayoutRow, TabControl.
{% endhint %}

{% hint style="success" %}
Não se preocupe com os detalhes técnicos, o Gvinci cuida disso para você, tendo apenas que arrastar e soltar os controles na tela para que ele cuide do código necessário para uma exibição responsiva, que se molda ao tamanho da tela do dispositivo usado para acessar sua aplicação.
{% endhint %}

### Habilita auto geração \(Experimental\)

Com a opção habilitada, cada vez que clicar no botão de salvar, com alterações feitas no design de uma página, a geração de código-fonte é feita automaticamente, atualizando o módulo alterado imediatamente. Assim, se usar o botão "[Roda projeto no browser](../../../../../botoes/barra-de-ferramentas/botao-roda-projeto-no-browser.md)", sua aplicação será carregada e novas atualizações que realizar e salvar, sem fechar o navegador, refletirão essas modificações imediatamente, sem necessidade de geração completa de códigos-fonte de toda a solução.

### Tipo de módulo para vínculo com templates

É possível selecionar alguns tipos de módulos padrão do Gvinci para receberem templates específicos através do painel [Template Manager](../../../untitled-1/template-manager/).

![](../../../../../.gitbook/assets/image%20%2858%29.png)

Com isso, o módulo pode manter sua função específica para o projeto e ainda ser vinculado a um template já gravado de modo a facilitar a confecção de tela para esses módulos.

![](../../../../../.gitbook/assets/image%20%2862%29.png)

### Descrição

Campo de conteúdo livre destinado a anotações pertinentes ao módulo com objetivo de documentação.



