# Gvinci : Propriedades do Grid

O controle **Grid** apresenta as propriedades conforme imagens abaixo:

![](http://www.gvinci.com.br/manual/8_085.zoom80.png)   ![](http://www.gvinci.com.br/manual/8_086.zoom80.png)   ![](http://www.gvinci.com.br/manual/8_087.zoom80.png)   ![](http://www.gvinci.com.br/manual/8_088.zoom80.png)

Além das [propriedades comuns dos controles](http://www.gvinci.com.br/manual/propriedades_comuns_de_control.htm), destacamos as específicas deste controle:

**• Aparência**  
     **• Columns:** Permite incluir colunas no Grid  
     **• NoRowsMsg:** Exibe uma mensagem quando Grid estiver sem registros para apresentar  
**• Comportamento**  
     **• AllowColumnRezise:** Permite redimensionar as colunas na aplicação final  
     **• AllowColumnsReorder:** Permite reposicionar as colunas na aplicação final  
     **• AllowDelete:** Permite que os dados do Grid sejam apagados pelo usuário

Observe, na figura abaixo, o botão **"Delete"** sendo exibido quando o valor desta propriedade é **True**.

![](http://www.gvinci.com.br/manual/allowdelete-yes.png)

**• AllowExportToCsv:** Habilita a exportação para arquivo Csv  
**• AllowExportToExcel:** Habilita a exportação para arquivo Excel  
**• AllowExportToPdf:** Habilita a exportação para arquivo Pdf  
**• AllowExportToWord:** Habilita a exportação para arquivo Word  
**• AllowFilteringByColumn:** Ativa o filtro por coluna  
**• AllowGrouping:** Permite que as colunas sejam agrupadas:

![](http://www.gvinci.com.br/manual/allowgroupinggv5.zoom71.png)

**• AllowInsert:** Ativa e desativa a exibição do botão "Adicionar", em destaque na figura abaixo. Este recurso permite que um novo item seja adicionado ao Grid, durante a execução da aplicação

![](http://www.gvinci.com.br/manual/allowinsert-yes.png)

**• AllowKeyboardNavigation:** Permite a navegação pelo grid através do teclado  
**• AllowPaging:** Ativa a paginação do Grid

![](http://www.gvinci.com.br/manual/allowpaginggv5.zoom64.png)

**• AllowRowResize:** Permite redimensionar a altura das linhas do grid  
**• AllowScroll:** Ativa e desativa a rolagem no Grid na aplicação gerada  
**• AllowSelectionCheckBoxes:** Permite o uso de caixas de seleção no Grid  
**• AllowSorting:** Habilita a classificação de dados do Grid  
**• AllowUpdate:** Ativa e desativa a exibição do botão "Editar". Este botão é utilizado para fazer a alteração dos itens do Grid.

![](http://www.gvinci.com.br/manual/allowrefresh-yes.png)

**• DeleteGridValidation:** Permite definir uma condição para deletar o registro no grid  
**• ExportToNexWindow:** Ativa a exportação para uma nova janela  
**• FrozenColumns:** Define o número de colunas que permanecerão fixas à esquerda  
**• InsertGridValidation:** Permite definir uma condição para inserir registros no grid  
**• InsertItemPageIndexAction:** Controla a exibição de item para indexação de página do Grid  
**• ShowPagerSizes:** Mostra controle para que o usuário escolha quantos itens serão listados por página  
**• UpdateGridValidation:** Permite definir uma condição para alterar o registro no grid

**• Dados**

**• EditMode:** Permite alterar o modo de edição do Grid

![](http://www.gvinci.com.br/manual/editmodegv5.png)

**• FieldsKey:** Define campos para ordenação, caso a tabela escolhida seja uma View \(Visão / Exibição\)  
**• ParentGrid:** Permite definir um Grid-pai para o Grid atual quando há mais de um Grid na mesma página.  
**• Relation:** Exibe a quantidade de relacionamentos com o Grid. Ao clicar no botão é aberta a janela Definição de Relacionamento, para relacionar os campos entre as tabelas.  
Para detalhes, consulte o tópico Relacionamento no Grid.  
**• Layout**  
**• CommandItemDysplay:** Define a exibição da barra de comandos  
**• Pagesize:** Determina a quantidade de linhas por página  
**• StyleMode:** Permite definir como será a contagem das páginas  
**• TableBehavior:** Determina se o Grid terá tamanho fixo \(Fixed\) ou se poderá ser redimensionado \(Normal\)

