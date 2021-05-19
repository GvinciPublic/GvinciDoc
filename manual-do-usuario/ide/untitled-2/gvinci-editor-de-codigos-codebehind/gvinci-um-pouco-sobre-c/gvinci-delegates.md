# Delegates

**Delegate** \(representante\) é uma classe especial que funciona como ponteiro para funções. Ao criarmos uma instância de um delegate, passamos ao construtor o nome da função que desejamos referenciar.

   
//Cria um delegate 

delegate void MeuDelegate\(int a, int b\); 

O código acima cria um delegate que recebe dois inteiros como parâmetro, ou seja, esse delegate só poderá apontar para uma função que tenha a mesma assinatura, como a seguinte:

            void MinhaFuncao\(int a, int b\);

           Para o delegate referenciar a função acima, devemos escrever:

             MeuDelegate instanciaDoDelegate = new MeuDelegate\(MinhaFuncao\);  
 

Agora instanciaDoDelegate aponta para MinhaFuncao e se chamarmos instanciaDoDelegate\(1,2\); a MinhaFuncao\(1,2\) será executada.

Um delegate pode referenciar uma ou mais funções. Uma maneira de se fazer isso é:  
   
MeuDelegate instanciaDoDelegate = new MeuDelegate\(funcao1\);  
instanciaDoDelegate += funcao2;  
instanciaDoDelegate += funcao3;   
 

Um delegate representa a assinatura de um método, podendo ser ele anônimo \(utilizado em rotinas de ordenação, por exemplo\), ou a assinatura de um método de evento.  
 

Em **C\#** os delegates são controles de primeira classe, totalmente suportados pela linguagem, um delegate é um tipo de referência usado para encapsular um método como uma assinatura e um tipo de retorno específico. Você pode encapsular qualquer método usando um **delegate,** mas o método deve coincidir com o delegate usado.

Criamos um delegate com a palavra-chave delegate seguida de um tipo de retorno e a assinatura dos métodos que podem ser delegados a ela, conforme abaixo:

public delegate int delegateInteiro\( \);

Esta declaração define um delegado chamado delegateInteiro, que encapsulará qualquer método que retorne um inteiro.

Uma vez definido o delegado, você pode encapsular um método-membro com ele, instanciando-o e passando um método que coincida com o tipo de assinatura.

Os eventos em **C\#** são introduzidos com os delegates.

