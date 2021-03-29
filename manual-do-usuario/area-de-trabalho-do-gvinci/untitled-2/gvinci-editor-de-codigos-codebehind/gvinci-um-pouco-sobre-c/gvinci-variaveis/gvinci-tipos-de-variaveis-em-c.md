# Tipos de variáveis em C\#

As variáveis na linguagem **C\#** podem ser dos seguintes tipos:

| Tipo | Valores |
| :--- | :--- |
| bool | Verdadeiro ou Falso \(Valores booleanos\) |
| byte | 0 a 255 \(8 bits\) |
| sbyte | -128 a 127 \(8 bits\) |
| char | Um caractere \(16 bits\) |
| decimal | ± 1.0 × 10−28 a ±7.9 × 1028 \(128 bits\) |
| double | ± 5.0 × 10−324 a ±1.7 × 10308 \(64 bits\) |
| float | ± 1.5 × 10−45 a ±3.4 × 1038 \(32 bits\) |
| int | -2,147,483,648 a 2,147,483,647 \(32 bits\) |
| uint | 0 a 4,294,967,295 \(32 bits\) |
| long | – 9,223,372,036,854,775,808 a 9,223,372,036,854,775,807 \(64 bits\) |
| ulong | 0 a 18,446,744,073,709,551,615 \(64 bits\) |
| object | Qualquer tipo. |
| short | -32,768 a 32,767 \(16 bits\) |
| ushort | 0 a 65,535 \(16 bits\) |
| string | Sequência de caracteres \(16 bits por caractere\) |

Todos os tipos na tabela com exceção dos tipos object e string são conhecidos como tipos simples.

Para retornar o tipo de qualquer variável do C\# você pode usar o método GetType\( \); Como no exemplo:

Console.WriteLine\(minhaVariavel.GetType\(\)\); 

Isso retornaria o tipo da variável minhaVariavel.

