# Gvinci : Processos

A definição de processos é semelhante à definição de lançamentos, explicada no item anterior. A principal diferença é que, no lançamento, um registro novo é criado na tabela alvo e seus campos são modificados. Já no processamento, um registro deve ser localizado e posicionado na tabela alvo para que um ou mais campos sejam modificados.

![](http://www.gvinci.com.br/manual/processos-tela.zoom84.png)

Os passos para a definição de um processo são os seguintes:

**1.** Clique sobre o botão ![](http://www.gvinci.com.br/manual/adicion1gv5.png) para criar um novo processo;

**2.** Identifique o processo, preenchendo o campo de nome **Título;**

**3.** Selecione o **campo-alvo**, ou seja, um campo da tabela-alvo que receberá o processo;

**4.** Se necessitar, você poderá executar o processo em definição antes que os dados sejam gravados efetivamente, marcando a opção **Executar antes de gravar o registro efetivamente.**

Essa opção oferece possibilidades sobre a execução do processo que pode ser efetuado antes da primeira atualização \(update\) da tabela básica. Essa opção é habilitada somente se o processo for efetuado sobre a tabela básica da janela de dados.

**5.** **Condição para fórmula direta** estabelece uma condição para que o processo seja efetivado. Esta condição pode ser estabelecida utilizando-se os mesmos recursos existentes para a **criação** das validações e pré-validações. Uma vez estabelecida uma condição, o processo só será executado quando esta condição for atendida;

**6.** Informe, no campo **Fórmula direta**, uma fórmula ou expressão para ser inserida no campo-alvo durante a inclusão de registros na tabela básica;

**7.** Se precisar de uma condição para executar a fórmula inversa, utilize o campo **Condição para fórmula inversa;**

**8.** No campo **Fórmula inversa** você pode colocar uma expressão que somente será executada quando os registros da tabela básica forem excluídos. Esta fórmula ou expressão deverá ser exatamente a inversa da fórmula direta para desfazer ou anular completamente a operação efetuada por ela.

Para apagar as definições de um processo, basta selecionar o processo desejado na lista, clicar sobre o botão ![](http://www.gvinci.com.br/manual/excluibtgv5.png) e confirmar a retirada. Quando existir mais de um processo, a ordem de execução é determinada pela ordem na lista de processos.

Vídeos explicativos disponíveis pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[10.1 - Gvinci Processo em página de dados - Básico](https://www.youtube.com/watch?v=m-4yW0pQu4U)

[10.2 - Gvinci Processo em Página de dados com uma condição](https://www.youtube.com/watch?v=L84mV4Kakb4)

[10.3 - Gvinci Ordem de processo e lançamento](https://www.youtube.com/watch?v=F-mquE5oeMc)

[13.1 - Criando processo em Grid - Tabela Auxiliar](https://www.youtube.com/watch?v=4k72LjPg8UU)

[13.2 - Gvinci Criando Processo no Grid - Básico](https://www.youtube.com/watch?v=REg-Ru0DmKw)

[13.3 - Processo em Grid com condição](https://www.youtube.com/watch?v=-ZcMTm3FkVc)

