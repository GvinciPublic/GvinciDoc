# Comportamento

**AcceptBlankText / Texto em Branco:** Ao ativar esta propriedade \(True\), você permitirá que o controle fique sem exibir nenhum item.

**AllowFileExtensions:** Permite definir quais serão as extensões aceitas pelo controle.

![](http://www.gvinci.com.br/manual/allowfileextensions.png)

**AssociatedPager / Pager Associado:** Permite inserir um nome do Pager associado

**AutoCryptDecrypt / Encriptar:** Ativa e desativa o modo automático de criptografia e descriptografia do conteúdo do controle

**AutoPostBack:** Ativa e desativa o modo automático de PostBack, que é o processo de envio de informações através de controles da página atual para ela mesma, a fim de que essas informações possam ser processadas pela própria página.

**Clip / Limitar na Borda:** Ativar e desativar a exibição do excedente do conteúdo, quando o conteúdo ultrapassar os limites da área do Div.

**CollapseAnimationDuration ou HideAnimationDuration / Tempo de Animação \(Fechar\):** Determina o tempo de duração do efeito ao fechar o controle.

**CollapseAnimation-Type ou HideAnimation-Type / Tipo de Animação \(Fechar\):** Qual tipo de animação será definido ao fechar o controle.

**CollapseDelay / Duração do Recolhimento:** Define a duração do fechamento do menu.

**Cursor:** Permite alterar o estilo do ponteiro do mouse. O estilo selecionado nesta propriedade será aplicado quando o ponteiro do mouse parar sobre o controle durante a execução da aplicação.

![](http://www.gvinci.com.br/manual/cursortypes.png)

**DisplayType:** Determina o tipo para o botão:

**• ImageOnly:** Permite somente a inserção de imagem no botão  
**• TextOnly:** Somente texto no botão  
**• TextImage:** Permite que o botão contenha texto e imagem ao mesmo tempo

**Esta propriedade está disponível somente quando o botão é inserido em uma barra de ferramentas \(toolbar\).**

**DisableOnNavigation / Desabilita em Navegação:** Habilita e desabilita o uso do controle durante a navegação. É utilizada para que o controle seja desabilitado quando a página estiver em modo de navegação, ou seja não estiver sendo editada ou em momento de inclusão de registros. A página estará em modo de navegação se as propriedades da página em destaque abaixo \(exceto Mobile\) forem desmarcadas:

![](http://www.gvinci.com.br/manual/desmarqpropgv5.zoom90.png)

**EnableAutoScroll / Rolagem Automática:** Habilita rolagem automática.

**Enabled / Habilitar:** Habilita \(True\) ou desabilita o controle \(False\) durante a execução da aplicação.

**EnableEmbeddedSkins / Habilitar Skins:** Ativa o uso dos skins disponibilizados na propriedade Skin.

**EnableLoadOnDemand / Carregar por Demanda:** Ativa ou desativa o envio de um "callback" - requisição para atualização da página - para o servidor quando um usuário final alterar o valor do Combo. Isso permite que o conteúdo do combo seja exibido imediatamente de acordo com o que é digitado. Quando o usuário pressionar a tecla "A", por exemplo, os itens que comecem com a letra "A" serão imediatamente exibidos.

**ExpandAnimationDuration ou ShowAnimationDuration / Tempo de Animação \(Abrir\):** Determina o tempo de duração do efeito ao abrir o controle.

**ExpandAnimation-Type ou ShowAnimation-Type/ Tipo de Animação \(Abrir\):** Qual tipo de animação será definido ao abrir o controle.

**InitialValue / Valor Inicial:** Define um valor inicial para o controle. Ao clicar no botão extensor desta propriedade, a janela Fórmula é exibida. Nesta janela, são exibidos parâmetros, variáveis, apelidos e nomes de campos que podem ser utilizados como valor inicial.

![](http://www.gvinci.com.br/manual/formulajanel.zoom69.png)

**LoginVisibility / Visibilidade Pelo Login:** Define se o controle será visível de acordo com a autenticação.

**• Always:** Será visível sempre, independente de estar logado ou não  
**• OnlyLoggedIn:** Será visível apenas quando o site estiver logado;  
**• OnlyLoggedOut:** Será visível apenas quando o site não estiver logado

**Mask:** Define uma máscara para a exibição da data no controle.

**ReadOnly:** Determina que o controle seja somente leitura, não permitindo alteração.

**RefreshConditionalProperties / Atualizar Propriedades Condicionais:** Atualiza as fórmulas utilizadas. Apresenta três opções:

**• Client:** Atualiza as fórmulas somente na plataforma do cliente \(navegador\);  
**• Server:** Atualiza as fórmulas somente na plataforma do server \(servidor\);  
**• ClientServer:** Atualiza as fórmulas usadas na plataforma do cliente e do servidor ao mesmo tempo.

**RefreshFilterCombo:** Atualiza o filtro de todos os controles ComboBox.

**RenderMode:** Permite escolher entre os modos de renderização, entre:

**• LightWeigth:** Modo leve de carregamento  
**• Auto:** Permite a escolha automática pelo sistema entre os modos  
**• Classic:** Preserva a renderização original, mais completa  
**• Native:** Modo nativo de carregamento  
**• Mobile:** Adapta-se melhor ao ambiente mobile, como toque e tamanhos de fontes e controle

**Show AjaxLoading / Mostrar AjaxLoading:** Torna visível o AjxLoading.

**TabIndex / Ordem de Tabulação:** Estabelece a sequência de acesso aos controles na tela, quando o usuário pressiona a tecla **&lt;Tab&gt; ou &lt;Enter&gt;.** Para exibir o valor desta propriedade no interior do controle, utilize o atalho: **&lt;Ctrl&gt; + &lt;Shift&gt; + &lt;T&gt;.**

**ToolTip / Texto de Ajuda:** Utilize esta propriedade para inserir uma Hint - mensagem descritiva da função do controle que será apresentada quando o ponteiro do mouse for posicionado sobre o controle durante a execução da aplicação.

**Validation:** Expressão ou função em C\# que retorna um valor lógico \(True ou False\), indicando se a informação digitada no controle é válida. Esta condição é avaliada quando o usuário clica sobre o botão de gravação ou de prosseguir \(forms sem vinculação direta com dados\). Para mais detalhes, veja **validação**.

**Visible / Visibilidade:** Permite que o controle seja visível \(True\) ou oculto \(False\).

