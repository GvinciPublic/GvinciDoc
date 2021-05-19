# Lançamentos

Os lançamentos são utilizados em tabelas estrangeiras a partir da digitação de informações em outras tabelas, inclusive com o estabelecimento de condições para que lançamentos sejam criados \(neste caso, sob a condição do registro não existir na tabela\).

No lançamento, novos registros são inseridos na tabela-alvo e seus campos imediatamente modificados com os valores estabelecidos, não havendo a necessidade de existir relacionamento entre as tabelas. No entanto, mesmo assim é necessário que esta tabela seja informada nas **Tabelas Auxiliares.**

As aplicações geradas pelo **Gvinci** são capazes de controlar não só a geração desses lançamentos como também a sua manutenção. Vamos ver, agora, como é que a aplicação controla quais registros foram gerados por meio de lançamentos e a partir de qual arquivo foram originados.

Sempre que um lançamento é definido no projeto, dois campos podem ser designados para controle dos lançamentos, na definição da estrutura da tabela:

 •Um campo que servirá como INT~LAN é criado dentro da tabela geradora do lançamento para servir de ligação com o registro lançado na tabela alvo. Este campo vai controlar quantas vezes o lançamento é feito.

   •Um campo que servirá de COD~LAN é criado dentro da tabela alvo do lançamento. Este campo vai controlar quantos registros foram gerados através do lançamento recebido. 

![](http://www.gvinci.com.br/manual/intlan1.zoom77.png)

Se você relacionou uma ou mais **tabelas auxiliares**, a interface representada pela figura abaixo estará habilitada para a definição de lançamentos.

![](http://www.gvinci.com.br/manual/lancamento511.zoom77.png)

Para criar um lançamento em uma tabela auxiliar, proceda conforme se segue:

**1.** Clique sobre o botão ![](http://www.gvinci.com.br/manual/adicionar.png) para criar um novo Lançamento;

**2.** Digite uma identificação para o lançamento no campo denominado Título;

**3.** Informe a quantidade de lançamentos que serão efetuados. Observe que este valor pode ser informado de diversas formas:

• Informando diretamente um número;  
• Informando uma variável que tenha criado e designado;  
• Capturando um campo qualquer do banco de campos;  
• Informando uma fórmula que envolva um ou mais campos;  
• Abrindo a janela Fórmulas através do botão , clicando no botão para elaborar uma função que retorne um valor a ser utilizado. Esta flexibilidade é útil, por exemplo, quando são efetuados diversos lançamentos em uma tabela, de acordo com o número de parcelas de pagamento de mercadorias.

**4.** Conforme o caso exigir, marque a opção **Excluir o lançamento quando registro gerador for excluído,** para que o **Gvinci** crie rotinas na aplicação final para apagar o registro alvo do lançamento, quando o registro que o gerou for apagado;

**5.** Se desejar, você pode estabelecer duas condições envolvendo o lançamento em definição:

Lembre-se que este lançamento só será executado após a inclusão do registro na tabela básica \(origem do lançamento\) razão pela qual deve-se ter cuidado especial sobre o modo como foi aberta esta tabela-alvo, na aba **Tabelas auxiliares.**

**6.** **Para executar o lançamento:** Preencha o campo **Condição de inclusão de lançamento**, clicando sobre o botão ![](http://www.gvinci.com.br/manual/adicionar.png),utilizando os mesmos recursos existentes para a criação das validações e pré-validações explicadas anteriormente neste tópico. Assim, o lançamento só será criado quando esta condição for atendida;

![](http://www.gvinci.com.br/manual/condicaolanc.zoom89.png)

**7.** **Para retirar o lançamento:** Preencha o campo **Condição de exclusão**, utilizando aqueles mesmos recursos. Assim, o lançamento só será retirado se esta condição for atendida;

**8.** Finalmente, fazendo uso da coluna **"Expressão a ser colocada no campo alvo",** para cada campo alvo, estabeleça uma expressão para processá-lo. Esta expressão pode ser definida utilizando-se a janela Fórmulas ou através do Editor de Códigos para elaborar uma função para retornar o valor desejado.

Vídeos explicativos disponíveis pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[11.1 - Gvinci Lançamento em página de dados - Básico](https://www.youtube.com/watch?v=lWpaeGrjT3c)

[11.2 - Gvinci Lançamento em Página de dados - Avançado](https://www.youtube.com/watch?v=hSTZh5lH0kk)

[14.1 - Gvinci Criando lançamentos em Grid - Básico](https://www.youtube.com/watch?v=n7NMwgWMI4c)

[14.2 - Gvinci Lançamento no Grid - Avançado](https://www.youtube.com/watch?v=L6WLkJmXdHE)

