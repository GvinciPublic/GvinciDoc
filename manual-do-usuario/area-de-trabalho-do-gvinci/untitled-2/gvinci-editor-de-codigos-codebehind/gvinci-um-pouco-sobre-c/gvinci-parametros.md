# Gvinci : Parâmetros

Os parâmetros permitem que se defina sobre quais dados a função deve operar.

**A função sound\(freq\),** por exemplo, recebe como parâmetro a frequência do som a ser gerado, permitindo que se defina seu comportamento a partir deste valor.

Para definir os parâmetros de uma função o programador deve explicitá-los como se estivesse declarando uma variável, entre os parênteses do cabeçalho da função. Caso precise declarar mais de um parâmetro, basta separá-los por vírgulas. No exemplo a seguir temos a função **SOMA** que possui dois parâmetros, sendo o primeiro um **floate** o segundo um **int.**

void SOMA\(float a, int b\)         // basta separar por vírgulas  
{  
 float result;                 // a declaração de variáveis é igual ao que   
                                 // se faz na função main   
 result = a+b;  
 printf\("A soma de %6.3f com %d é %6.3f\n, a,b,Result\);   
}

