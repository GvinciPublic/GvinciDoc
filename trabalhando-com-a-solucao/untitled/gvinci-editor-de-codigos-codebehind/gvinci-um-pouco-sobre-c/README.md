# Gvinci : Um pouco sobre C\#

Neste tópico apresentamos noções gerais de programação, bem como conhecimentos básicos da linguagem **C\#.** Por ser ambiente novo, comparado ao Desktop, o ambiente Web por vezes traz termos novos e típicos de componentes específicos. Será sempre de bom alvitre adquirir mais conhecimento a respeito da linguagem ou de seus auxiliares, tais como Ajax, JavaScript, ASPX, CSS, HTML, etc.

Para inserir comentários no código:

| • | **Várias linhas: utilize os caracteres "/\*" no início e "\*/" no final.** |
| :--- | :--- |


| **•** | **Uma linha: Utilize duas barras: "//" no início do comentário.** |
| :--- | :--- |


Para importar uma biblioteca, utilize a palavra **"Using"** antes do nome da biblioteca.

**Exemplo:**

Using System

No final de cada linha de instrução é necessário colocar **";"** \(ponto-e-vírgula\).

**Main** é um único método. Indica onde o programa pode ser executado. É uma entrada necessária para iniciar a execução.

O modificador static é usado para declarar um membro estático, que pertence ao próprio tipo e não a um controle específico. Você pode utilizar **static** com classes, campos, métodos, propriedades, operadores, eventos e os construtores.

**Void** especifica que o método não retorna valor algum \(nulo\), quando for preciso utilizar em um **Return.**

Os métodos ficam dentro de classes, no exemplo abaixo a classe é chamada "mensagem".

Para iniciar e encerrar um código, são usadas chaves { }.

**/\*** 

**\* aqui está meu primeiro programa**

**\* em linguagem C\#**

**\*/** 

**Using System;** 

**class Mensagem**

**{**  
         **// Método principal**

 **static void Main\(\)** 

 **{**  
                 **System.Console.WriteLine\("Já estou programando!!"\);**  
         **}**  
 **}** 

Vídeos explicativos disponíveis pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[KB02 - Multi-Empresa](https://www.youtube.com/watch?v=QcLg7FblhTk)

[KB04 - Cálculo de Idade](https://www.youtube.com/watch?v=is0-erFc04s)

[KB08 - PegaSequencia](https://www.youtube.com/watch?v=GkVQlmNC3JE)

[KB15 - URL como link no repeater](https://www.youtube.com/watch?v=Mm8abhjCUWo)

[KB38 - Somando dias a uma data com código em C\#](https://www.youtube.com/watch?v=RmCWic5WsN4)

[KB40 - Filtro em combobox por código C\#, usando campo da tabela de parâmetros.](https://www.youtube.com/watch?v=feWEE2hB2rE)

