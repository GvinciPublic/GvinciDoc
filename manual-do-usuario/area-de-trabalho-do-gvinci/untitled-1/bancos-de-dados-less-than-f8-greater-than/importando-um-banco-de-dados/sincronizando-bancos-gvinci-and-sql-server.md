# Sincronizando bancos - Gvinci & SQL Server

A sincronização de bancos existe para que os bancos, quando abertos, sejam atualizados conforme as alterações que são feitas. Por exemplo, se o banco estiver aberto em **SQL** e no **Gvinci,** qualquer alteração feita no banco será visualizada nesses dois programas.

**1.** Crie uma nova solução.

**2.** Abra o painel **Banco de Dados**, clicando no botão ![](http://www.gvinci.com.br/manual/bferr9gv5.png) ;

**3.** Clique no botão **"Importar do Banco"** ![](http://www.gvinci.com.br/manual/imp2bdgv5.png).

![](http://www.gvinci.com.br/manual/importbdbt3gv5.zoom100.png)

**4.** Preencha os dados para localização do banco, na caixa que aparecerá, conforme a figura abaixo:

![](http://www.gvinci.com.br/manual/localbdextgv5.zoom100.png)

**5.** Clique no botão ![](http://www.gvinci.com.br/manual/carregarbtgv55.png).

**6.** Repita novamente os passos **3, 4** e **5**. Após clicar em ![](http://www.gvinci.com.br/manual/carregarbtgv55.png), aparece a mensagem abaixo:

![](http://www.gvinci.com.br/manual/sincroniza.zoom80.png)

**7.** Clique em ![](http://www.gvinci.com.br/manual/sincronizar-bt.png). O quadro abaixo será exibido:

![](http://www.gvinci.com.br/manual/sincronizabdgv5.zoom80.png)

Na seção **Estrutura Sincronizada** é exibida a estrutura original do banco, conforme gravada no servidor SQL. Na seção **Estrutura Atual** é exibida a estrutura do banco cuja solução está aberta no **Gvinci.**

Para cada alteração efetuada, uma cor diferente é atribuída. Observe a legenda de cores:

![](http://www.gvinci.com.br/manual/sincronizacores411.png)

**• Incluído:** O item será adicionado na estrutura do banco no **Gvinci;**  
**• Alterado:** O item será modificado de acordo com a estrutura importada;  
**• Ignorado:** O item será ignorado e não será criado no Gvinci. Esta opção é executada após clicar no botão "Reverter";  
**• Excluído:** O item existente no Gvinci será excluído.

Para aceitar as alterações feitas, clique em ![](http://www.gvinci.com.br/manual/aplicarsincronia411.zoom69.png).

Caso queira desfazer a alteração, ignorando as alterações para o item selecionado, utilize o botão ![](http://www.gvinci.com.br/manual/revertersincronia411.zoom64.png).

