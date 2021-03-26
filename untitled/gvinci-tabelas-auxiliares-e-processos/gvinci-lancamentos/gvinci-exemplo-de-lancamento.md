# Gvinci : Exemplo de lançamento

Este lançamento terá como tabela **ORIGEM a TB\_VENDAS** e como tabela **ALVO a TB\_CONTAS\_RECEBER.** Isso significa que novos registros serão criados na tabela **TB\_CONTAS\_RECEBER** cada vez que o lançamento for executado.

Na tabela **TB\_VENDAS,** teremos um campo que irá buscar o valor na tabela **TB\_VENDEDOR.** Este campo "Vendedor" que terá como controle um ComboBox na página Vendas.

![](http://www.gvinci.com.br/manual/vendedor22.png)

**1.** Crie a tabela **TB\_VENDEDOR** de acordo com os campos abaixo:

![](http://www.gvinci.com.br/manual/tbvendedor1.png)

**2.** Defina as propriedades dos campos conforme a tabela:

| Nome | Título | Tipo | Tamanho | Permitir Nulo | Decimal | Máscara |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| VE\_ID | Código | Numérico | 10 | NÃO MARCAR | - | 9999999999 |
| VE\_NOME | Nome | Caracter | 40 | NÃO MARCAR | - | @! |

**3.** Crie uma tabela **TB\_VENDAS** com os campos abaixo:

![](http://www.gvinci.com.br/manual/tbvendas1.png)

**4.** Defina as propriedades dos campos conforme a tabela:

| Nome | Título | Tipo | Tamanho | Permitir Nulo | Decimal | Máscara |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| VEN\_ID | Código | Numérico | 10 | NÃO MARCAR | - | 9999999999 |
| VEN\_DATA | Data | Data | - | NÃO MARCAR | - | dd/MM/yyyy |
| VEN\_VENDEDOR | Vendedor | Caracter | 40 | NÃO MARCAR | - | @! |
| VEN\_VALOR | Valor | Numérico | 10 | NÃO MARCAR | 2 | 99.999.999,99 |
| VEN\_VENCIMENTO | Vencimento | Data | - | NÃO MARCAR | - | dd/MM/yyyy |

O índice desta tabela será o campo **VEN\_ID,**  portanto, marque a opção **"Sequencial".**

**5.** Clique com o botão direito sobre a tabela e crie uma página de dados com os campos marcados conforme abaixo:

![](http://www.gvinci.com.br/manual/escolhaoscam.png)

**6.** Posicione os campos de modo a deixar o design semelhante à figura abaixo:

![](http://www.gvinci.com.br/manual/vendasdesign.png)

**7.** Crie uma tabela chamada **TB\_CONTAS\_RECEBER,** com os campos mostrados abaixo:

![](http://www.gvinci.com.br/manual/tbcontasrec.png)

**8.** Preencha as propriedades dos campos conforme abaixo:

| Nome | Título | Tipo | Tamanho | Permitir Nulo | Decimal | Máscara |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| REC\_ID | Código | Numérico | 10 | NÃO MARCAR | - | 9999999999 |
| VEN\_ID | Código Venda | Numérico | 10 | MARCAR | - | 9999999999 |
| REC\_VENCIMENTO | Vencimento | Data | - | NÃO MARCAR | - | dd/MM/yyyy |
| REC\_VALOR | Valor | Numérico | 10 | NÃO MARCAR | 2 | 99.999.999,99 |

**9.** Clique com o botão direito sobre a tabela e crie uma página com Grid com os campos marcados conforme abaixo:

![](http://www.gvinci.com.br/manual/camposrec.png)

A página com **Grid** ficará semelhante à figura abaixo:

![](http://www.gvinci.com.br/manual/contasrecebgrid.png)

A tabela **TB\_VENDAS** será a origem do lançamento. Os lançamentos são inseridos na seção de Tabelas auxiliares da página.

**10.** Selecione a página **VENDAS** e clique em **Tabelas Auxiliares**, na parte inferior do design.

![](http://www.gvinci.com.br/manual/tabauxiliarvend.png)

O lançamento precisará de um tabela **ALVO**, ou seja, a tabela onde serão criados os registros do lançamento. Por isso, vamos adicionar a tabela T**B\_CONTAS\_RECEBER** como tabela auxiliar.

**11.** Clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png) para inserir a tabela auxiliar:

![](http://www.gvinci.com.br/manual/addtbaux.zoom84.png)

**12.** Em **"Tabela",** selecione **TB\_CONTAS\_RECEBER:**

![](http://www.gvinci.com.br/manual/tbtable.png)

**13.** Clique na aba **"Lançamentos" e no botão** ![](http://www.gvinci.com.br/manual/adicionar.png):

![](http://www.gvinci.com.br/manual/addlanc.png)

O **Gvinci** pode criar um campo para controle de lançamentos, chamado **COD\_LAN.** Neste campo é armazenada uma sequência de números que identificam o lançamento no banco de dados. A criação deste campo não é obrigatória. A seguinte pergunta irá aparecer.

![](http://www.gvinci.com.br/manual/codlannao.zoom64.png)

**14.** Clique em **"Sim"** e o campo **COD\_LAN** será criado, porém, só será preenchido de forma automática quando o lançamento for feito.

**15.** Insira o título para o lançamento.

**16.** Insira a quantidade de registros que serão criados na tabela **TB\_CONTAS\_RECEBER.** Neste exemplo, nosso lançamento irá criar somente um registro, portanto, colocamos **"1".**

![](http://www.gvinci.com.br/manual/quantlanca.png)

**17.** Mantenha marcada a opção de exclusão de lançamento e não será necessário preencher os campos de condição para inclusão e exclusão.

Os campos-alvos, ou seja, da tabela **ALVO** que é a tabela **TB\_CONTAS\_RECEBER,** são listados na coluna à esquerda e na coluna direita precisamos clicar no botão ![](http://www.gvinci.com.br/manual/adicionar.png) para inserir os campos correspondentes da tabela **ORIGEM,** da tabela **TB\_VENDAS.**

![](http://www.gvinci.com.br/manual/camposalvos.zoom101.png)

**18.** Clique no botão ![](http://www.gvinci.com.br/manual/adicionar.png) para inserir a expressão que será inserida em **VEN\_ID.**

![](http://www.gvinci.com.br/manual/rec2.png)

**19.** Dê um duplo clique em **\[AUX\_TB\_VENDAS\].\[VEN\_ID\]** e clique em ![](http://www.gvinci.com.br/manual/btok24.png).

![](http://www.gvinci.com.br/manual/auxvenid.zoom85.png)

**20.**  Clique em ![](http://www.gvinci.com.br/manual/adicionar.png) para inserir a expressão correspondente a **REC\_VENCIMENTO:**

![](http://www.gvinci.com.br/manual/rec3.png)

**21.** Dê um duplo clique em **\[AUX\_TB\_VENDAS\].\[VEN\_VENCIMENTO\]** para inserir este campo na seção de Expressão e clique em ![](http://www.gvinci.com.br/manual/btok24.png).

![](http://www.gvinci.com.br/manual/vencim.png)

**22.** Clique em ![](http://www.gvinci.com.br/manual/adicionar.png) para inserir a expressão correspondente a **REC\_VALOR:**

![](http://www.gvinci.com.br/manual/rec4.png)

**23.** Dê um duplo clique em \[**AUX\_TB\_VENDAS\].\[VEN\_VALOR\]** para inserir este campo na seção de Expressão e clique em ![](http://www.gvinci.com.br/manual/btok24.png).

![](http://www.gvinci.com.br/manual/vencvalor.png)

O resultado final deverá ser:

![](http://www.gvinci.com.br/manual/rec1.png)

Desta forma, o lançamento está configurado.

**24.** Na página Principal, crie os itens de menu para as páginas **CONTAS A RECEBER, VENDAS e VENDEDOR.** Em seguida, execute a aplicação.

Vídeos explicativos disponíveis pelo [Canal da SSI no youtube](https://www.youtube.com/user/SSITecnologia):

[11.1 - Gvinci Lançamento em página de dados - Básico](https://www.youtube.com/watch?v=lWpaeGrjT3c)

[11.2 - Gvinci Lançamento em Página de dados - Avançado](https://www.youtube.com/watch?v=hSTZh5lH0kk)

