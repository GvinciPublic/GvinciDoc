# Definindo solução

Toda solução deve ter no mínimo um projeto. A definição da solução geralmente é feita antes da definição do projeto.

Para definir as propriedades da solução, clique duas vezes sobre **"Título da solução"** na árvore da solução**.**

![](../../.gitbook/assets/image%20%2833%29.png)

Será aberta a tela de "Definição da Solução", como abaixo:

![](../../.gitbook/assets/image%20%2820%29.png)

Preencha as propriedades com as informações necessárias:

### **Título**

Campo obrigatório, define um título para a solução. É possível também definir títulos em mais de um idioma para a aplicação clicando no botão ![](http://www.gvinci.com.br/manual/botaoidiomagv5.png), conforme destacado na imagem abaixo.

![](../../.gitbook/assets/image%20%287%29.png)

Em diversas outras propriedades de um projeto, encontrará possibilidade de se definir textos conforme os idiomas cadastrados para a solução. Ver "**Idiomas**", abaixo.

![](../../.gitbook/assets/image%20%2843%29.png)

### **Pasta da solução**

Define em que pasta a aplicação será gravada. Nessa pasta também serão gravados os projetos e todos os seus módulos dentro de subpastas. Observe a figura abaixo, exibindo as duas subpastas criadas dentro da pasta da solução \(Projeto e Components\), após a geração do código fonte da aplicação:

Dentro da pasta **Projeto** serão armazenados todos os itens referentes ao projeto, inclusive as subpastas exibidas no painel **Módulos da solução.** Para mais detalhes, consulte o tópico **Estrutura de um projeto.**

A pasta padrão sugerida é criada dentro de **&lt;pasta usuário windows&gt;\Documents\Gvinci Diamante.** Para detalhes, consulte o tópico [**Local da solução**](gvinci-local-da-solucao.md).

### **Chave de encriptação**

Permite inserir uma chave de encriptação a ser usadas em gravação e leitura de dados sensíveis que precisam ser protegidos de acesso não autorizado, como, por exemplo, as tabelas de controle de acesso, no banco de dados. Estas tabelas são responsáveis pelo controle de login e, portanto, deixar os dados como senhas sem qualquer forma de ocultação nas tabelas do banco de dados pode representar um grave risco de segurança.

Assim, as informações gravadas no banco de dados não serão legíveis até que ocorra uma decriptação dos dados usando essa chave.

A chave de encriptação também pode ser usadas em códigos manuais nas rotinas responsáveis pela encriptação e decriptação de informações.

{% hint style="danger" %}
De modo geral todo esse tratamento é feito de forma transparente ao usuário, ou seja, não requer intervenção direta de forma muito técnica, mas é de extrema importância que este campo seja alterado para uma chave de encriptação diferente da chave padrão para que não possa ser usada por terceiros para desproteger os dados com ela encriptados.
{% endhint %}

### **Versão da Solução**

O campo versão da solução tem a finalidade apenas de facilitar a identificação da solução na tela de abertura. A versão da solução não tem efeito de controle comportamental de nenhuma funcionalidade.

![](../../.gitbook/assets/image%20%2828%29.png)

Abaixo, tela de abertura da solução apresentando a versão definida do lado direito do título da solução. Observe ainda que muitas soluções da imagem não possuem informação alguma. Isso se dá pelo fato da propriedade versão não ter sido alterada.

![](../../.gitbook/assets/image%20%2838%29.png)

{% hint style="info" %}
O valor de versão definido é de sua livre escolha. O Gvinci não vai impedir que tenha 2 soluções com mesmo valor de versão. Observe também que para cada solução listada, ao lado esquerdo, existe um código numérico que é único, controlado pelo próprio Gvinci.
{% endhint %}

### **Idiomas**

Permite adicionar os idiomas que serão usados nos textos da aplicação gerada. Exemplo: português, espanhol, inglês.

Embora sejam listados inicialmente 3 idiomas, é possível adicionar outros mais, conforme necessidade, para que a aplicação gerada possa permitir que textos sejam "traduzidos" conforme o idioma selecionado.

![](../../.gitbook/assets/image%20%2824%29.png)

O idioma padrão, escolhido conforme imagem abaixo, refere-se ao idioma principal ou até único idioma para o caso de aplicações que não permitam a troca de idiomas. Nas propriedades de texto que permitem seleção de idioma, se não selecionados os idiomas para preenchimento de traduções, o texto definido será o texto usado na exibição da aplicação gerada.

![](../../.gitbook/assets/image%20%2826%29.png)

### **Controle de sequência manual**

Neste campo, poderá selecionar um banco de dados definido na solução, no qual serão criadas as tabelas de sistema responsáveis pelo controle dos valores de campos sequenciais.

![](../../.gitbook/assets/image%20%2846%29.png)

{% hint style="info" %}
O controle sequencial interno ao banco de dados é o recomendado para ser usado nas tabelas  dos banco de dados. Porém, são disponibilizados mecanismos que permitem um controle diferenciado sobre o controle dos valores dos campos sequenciais.
{% endhint %}

### **Components Namespace**

Permite inserir um nome de ambiente para os componentes de modo a organizar ou definir scopo das classes implementadas. Assim, os componentes usados no projeto usarão o namespace definido e suas implementações manuais poderão seguir a mesma estrutura organizacional para o caso de realizar codificações manuais.

Para mais detalhes, veja o tópico sobre [namespaces](https://docs.microsoft.com/pt-br/dotnet/csharp/programming-guide/namespaces/).

### **Utilizar banco de campos**

Ao preencher o nome do campo com um nome que já existe, as propriedades do primeiro campo criado são atribuídas a esse novo campo. Se desmarcar esta opção, não será possível atribuir as mesmas propriedades do campo que foi criado anteriormente. Esta opção é marcada automaticamente em uma nova solução.

![](../../.gitbook/assets/image%20%2832%29.png)

Para desativar esse recurso, desmarque a opção "**Utilizar banco de campos**" na tela de definição da solução

![](../../.gitbook/assets/image%20%2845%29.png)

### **Gerar Error List ao salvar**

A **Error List** \(Lista de erros\), está localizada no canto inferior da tela do Gvnici por padrão, bastando parar o mouse sobre ela ou clicar para que seja expandida, exibindo informações sobre erros encontrados na solução.

![](../../.gitbook/assets/image%20%2814%29.png)

Imagem abaixo exemplifica mensagem de erro sendo exibida em função da falta de definição de nome da página para um módulo chamado "**Formulários**".

![](../../.gitbook/assets/image%20%2834%29.png)

Com um duplo-clique sobre item da Error List o Gvinci tentará posicioná-lo no exato local onde a informação faltante se encontra.

A Error List é atualizada cada vez que ocorre gravação da solução ou quando é pressionado o botão "**Refresh**" no canto superior direito da janela com a lista de erros.

{% hint style="warning" %}
Apesar de ser um recurso muito importante, recomenda-se o uso da opção "Gerar Error List ao salvar" apenas na fase de aprendizado. A medida que a solução cresce muito, a varredura da solução por todas as propriedades a fim de localizar alguma inconsistência poderá causar lentidão do processo de gravação.
{% endhint %}

### **Framework alvo**

![](../../.gitbook/assets/image%20%2844%29.png)

Determina qual será o Framework \(plataforma\) utilizado pela aplicação. Como a aplicação gerada precisa ser hospedada em um servidor de páginas ASP.NET, é necessário que o código seja compatível com a versão do Framework que este servidor suporta. Então, defina o framework alvo conforme os requisitos do servidor onde hospedará sua aplicação.

{% hint style="success" %}
Se possível, mantenha sempre sua aplicação com a última versão disponível na listagem. Mas lembre-se de revisar essa propriedade no caso de sua aplicação funcionar normalmente no seu ambiente de testes e não funcionar a aplicação publicada.
{% endhint %}

### **Merge de DLLs ao publicar**

Ao marcar essa opção o Gvinci utilizará o mecanismo de pré-compilação para gerar um único arquivo .DLL a ser publicado, em vez de múltiplos arquivos .DLLs compilados para cada arquivo de conteúdo de interface de usuário web.

Para observar o resultado dessa alteração basta que após marcada a opção, clique no botão de "[Gerar arquivos para publicação](../../botoes/barra-de-ferramentas/ide-toolbar--botao-gerar-arquivos-para-publicacao.md)"

### **Habilita gerenciamento multi-desenvolvedor**

Para que seja possível o trabalho em equipe em uma mesma solução no Gvinci é necessário que cada módulo possa ser trabalhado individualmente para que não venha ocorrer problema de inconsistência na solução.

Ao habilitar esta opção, os módulos que estão em edição são marcados por um cadeado verde na árvore da solução, indicando que já existe um desenvolvedor trabalhando naquele módulo. Portanto, deverá evitar de abrir o módulo marcado.

Na imagem abaixo são exibidos cadeados para os módulos de cada janela aberta.

![](../../.gitbook/assets/image%20%2842%29.png)

Note agora, que só temos uma janela aberta \(Sobre\) e outros 2 módulos além do módulo "Sobre" estão marcados com o cadeado verde, indicando que os módulos foram abertos em outra instância do Gvinci e, portanto, deve evitar abri-los para edição.

![](../../.gitbook/assets/image%20%2823%29.png)

### **Descrição**

Permite inserir uma descrição detalhada da solução para documentação. Este campo é de uso livre, não afeta o comportamento da aplicação e poderá usá-lo com informações que o oriente com relação ao propósito da solução.

