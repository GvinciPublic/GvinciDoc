# Parâmetros

![](../../../../.gitbook/assets/image%20%2875%29.png)

É possível que na navegação para uma página, passemos valores a serem usados na nova página requisitada. Para isso, existem as query strings nas páginas ASP.NET. A query string é uma sintaxe usada na URL \(endereço da página\) de modo que além do nome da página a ser aberta, passamos também informações por meio de pares "Nome" e "valor" pela barra de endereços ou pelo link de abertura.

Dessa forma, se o caminho para uma página é http://www.meudominio.com.br/minhapagina.aspx e desejamos passar algumas informações que poderão ser usadas por essa página, acrescentamos um sinal de ? \(interrogação\) e seguimos com pares de "nomes" e "valores" unidos pelo símbolo & \(e comercial\).

Exemplo:

http://www.meudominio.com.br/minhapagina.aspx?campo1=valorcampo1&campo2=valorcampo2.

Dessa forma, a página minhapagina.aspx, poderá fazer uso dos valores informados na barra de endereço por meio do nome do campo definido na query string, ou seja, no Gvinci, definido na aba "Parâmetros".

Esse é o conceito por trás do recurso de parâmetros do Gvinci, disponível para módulos como: Página, Página de dados, Relatório, Relatório Telerik, Processo pré-definido e Email.

Com o Gvinci, sua preocupação será apenas definir um nome para o parâmetro, o tipo de dado que o parâmetro irá usar e se ele é opcional ou não. Todas as opções de uso de query strings \(parâmetros\), são feitas de forma prática e visual, sem necessidade de codificação manual.

**Opcional**

Ao marcar o checkbox opcional, o campo poderá ficar vazio, sem obrigatoriedade de preenchimento.

Cada parâmetro é adicionado ou removido da lista através dos botões + e -, respectivamente.

![](../../../../.gitbook/assets/image%20%2876%29.png)

### E depois que criamos os parâmetros?

O valor de cada um dos parâmetros pode ser usado internamente na página onde os definiu e será usado também nos eventos de navegação para a página que os possui.

Nas propriedades que permitem uso de fórmulas, como a propriedade "Text" de controles "Label", por exemplo, observará que aparecem além dos campos da tabela básica, [variáveis de ambiente customizadas](../../../trabalhando-com-a-solucao/definindo-projeto/), campos de tabelas de parâmetros, variáveis de sistema e os campos de parâmetros que vimos aqui como definir. Dessa forma, podemos usar os valores recebidos pela página, através da query string, ou seja, pela barra de endereço, para construir nossas fórmulas ou expressões de filtragens, por exemplo.

![](../../../../.gitbook/assets/image%20%2877%29.png)

O outro uso ocorrerá na página onde temos algum evento de navegação para a página que criamos os parâmetros.

Abaixo, definição de evento de navegação para página que tem 2 parâmetros definidos, identificados como "DataInicial" e "DataFinal". Na imagem, estão sendo passados valores fixos para os parâmetros definidos, mas poderiam ser também fórmulas definidas através do botão de + \(mais\) do lado direito do campo.

![](../../../../.gitbook/assets/image%20%2873%29.png)

Caso a página tenha permissões de "Permitir acesso direto pela URL", através da aba "Definitions" do módulo específico, também poderá usar a barra de endereços para passar diretamente os valores pretentidos, como na expressão abaixo:

http://www.meudominio.com.br/Pages/PaginaAspx.aspx?DataInicial=21/05/2021&DataFinal=22/05/2021



