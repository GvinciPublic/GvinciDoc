# Gvinci : Condições para validação

Sempre que habilitar a validação de um campo, você pode definir condições para analisar o conteúdo do campo e retornar um valor válido.

As condições são formadas por parâmetros \(campos, operadores e operandos\) que farão uma triagem do que é estritamente permitido para o campo em questão.

Quando você utiliza o botão de extensão ![](http://www.gvinci.com.br/manual/extensor-botao.png) da propriedade Validation, a tela abaixo é exibida, solicitando que os campos sejam preenchidos.

![](http://www.gvinci.com.br/manual/validation2gv5.zoom81.png)

Há dois tipos de validação disponíveis:  
      **• Validação de Servidor:** terá seu código em CSharp \(cs\) e será executada na plataforma onde a aplicação é armazenada  
      **• Validação de Cliente:** terá seu código em JavaScript \(js\) e será executada na plataforma Cliente, através de um navegador \(Browser\)  
  
Na Validação de Servidor, temos as seguintes opções:  
  
**Campo:** Insira o campo que receberá a validação, ou seja, o campo da tabela básica que terá seus dados analisados antes de prosseguir.  
  
**Operador:** Insira um operador apropriado para a condição de validação. Os seguintes operadores estão disponíveis:

![](http://www.gvinci.com.br/manual/operadores1112.png)  
**• == igual a**  
**• != diferente de**  
**• &gt; maior que**  
**• &gt;= maior ou igual**  
**• &lt; menor que**  
**• &lt;= menor ou igual**  
**• Like = Comparação**

**Segundo Operando:** Insira o campo que deverá ter seu valor igual ao do primeiro campo inserido.

Ao marcar a opção **OPERAÇÃO**, você pode especificar uma condição manual, escolhendo o campo que será analisado para validação do primeiro campo.

As outras opções: Requerido, Dia/Mês, Mês/Ano, CPF, CNPJ, Registro de lançamento e Cartão de crédito, se referem ao campo que for inserido na opção **"Campo".**

A opção **REQUERIDO** indica que o campo NÃO poderá ficar sem conteúdo. Após clicar no botão concatenar ![](http://www.gvinci.com.br/manual/adicionar.png),  a expressão montada é a seguinte:

=\(CheckNotEmpty\(Valor\)\)

Como resultado, na execução da aplicação teremos:

![](http://www.gvinci.com.br/manual/validation4.png)

Pode ser usada com a opção **"Negar condição"** marcada, assim, quando o campo estiver vazio a condição de validação será executada. Esta validação é inserida quando a página é criada automaticamente.

Na figura abaixo, podemos observar a validação aplicada ao campo Mes, com a opção REQUERIDO marcada, indicando que o campo não poderá ficar sem conteúdo durante a execução da validação, no momento de gravar \(salvar\) os dados na tabela. Após clicar no botão concatenar ![](http://www.gvinci.com.br/manual/adicion1gv5.png), a expressão é montada:

![](http://www.gvinci.com.br/manual/validation3gv5.zoom90.png)

A validação na plataforma **Cliente** apresenta as seguintes opções:

![](http://www.gvinci.com.br/manual/validation4gv5.zoom89.png)

Além das opções já citadas acima também utilizadas na plataforma Servidor, temos:

**EMail:** Ao utilizar esta validação, o conteúdo do campo deverá obedecer ao formato de endereço de email, por exemplo, [endereco@site.com.br](mailto:endereco@site.com.br).

**Somente Números:** Exige que o conteúdo do campo seja somente numérico.

O próximo tópico trata sobre **Pesquisa em Tabela \(PTab\).**

