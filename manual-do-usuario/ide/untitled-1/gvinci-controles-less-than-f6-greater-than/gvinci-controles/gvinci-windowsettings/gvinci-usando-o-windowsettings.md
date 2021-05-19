# Usando o WindowSettings

O controle **WindowSettings** é utilizado para armazenar em seu interior o controle Window.

![](http://www.gvinci.com.br/manual/windowsset1.png)

Também pode ser utilizado para a propriedade **NavigationReference** de outro controle, ou seja, quando é necessário o retorno à própria página após uma consulta em outra página ou tabela.

Um exemplo desse uso é a opção LookUp \(pesquisa\) de um TextBox: Ao pesquisar em outra tabela o conteúdo para aquele TextBox, é necessário que o TextBox tenha o WindowSettings definido na propriedade NavigationReference para que o foco possa retornar à página onde está o TextBox.

