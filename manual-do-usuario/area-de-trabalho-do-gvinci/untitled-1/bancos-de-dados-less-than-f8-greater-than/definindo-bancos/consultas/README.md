# Consultas

As consultas \(views\) são usadas para exibirem os dados de campos específicos da mesma tabela ou de tabelas diferentes. Não é possível editar dados de uma view.

Para criar uma consulta, proceda da seguinte maneira:

**1.** Abra o painel **Banco de Dados**, pressionando **&lt;Ctrl&gt; + &lt;D&gt;**  ou clicando no botão ![](http://www.gvinci.com.br/manual/bferr9gv5.png), na barra de ferramentas;

**2.** Clique duas vezes sobre o banco de dados onde a consulta ficará armazenada;

**3.** Clique sobre **Consultas** com o botão direito do mouse e escolha **"Nova Consulta"**;

![](http://www.gvinci.com.br/manual/novaconsgv5.zoom80.png)

**4.** Preencha as propriedades conforme as explicações abaixo:

![](http://www.gvinci.com.br/manual/propconsgv5.zoom80.png)

**Nome:** Insira o nome interno da consulta que será usado pela aplicação;

**Provider:** Insira o nome do provider para a consulta;

**Título:** Insira o título da consulta que vai aparecer na estrutura do banco de dados;

**Gerar script para a view:** Uma view é uma tabela virtual gerada a partir de um SELECT que seleciona campos específicos de uma ou mais tabelas.

Marcando esta opção você define se o script da view será gerado no banco SQL, isso vai facilitar a manutenção e sua execução será mais rápida pois o Banco de dados vai guardar a sua view em memória. Se não marcar esta opção, então a view será montada diretamente em sua aplicação porem sua velocidade de execução será mais lenta e você não terá a possibilidade de alterar sem atualizar novamente sua aplicação no servidor.

**View Script:** Caso a opção de **Gerar script** acima tenha sido marcada, o script aparecerá nesse quadro.

![](http://www.gvinci.com.br/manual/constrbtgv5.png) Abre a janela **Construtor de Consultas** que oferece opções de filtragem para a construção de uma fórmula que irá determinar como a consulta funcionará;

![](http://www.gvinci.com.br/manual/constrconsgv5.zoom88.png)

**Descrição:** Insira uma descrição sobre a finalidade da consulta.

