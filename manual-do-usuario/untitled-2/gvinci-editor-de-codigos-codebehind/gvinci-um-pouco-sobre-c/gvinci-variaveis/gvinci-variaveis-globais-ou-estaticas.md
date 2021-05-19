# Variáveis Globais ou estáticas

Em C\# não existe o conceito de variáveis globais, como existe em Visual Basic, onde podem ser utilizados os módulos. Caso seja necessário partilhar dados entre formulários, pode-se criar uma classe com as variáveis e declará-las como static.

O exemplo abaixo declara a variável estática "contador" do tipo integer e já recebe o valor 1 quando é declarada.

using System;

class MyClass

{

 public static int contador = 1;

 contador = contador + 1;

}

