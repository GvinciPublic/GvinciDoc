# Módulo: Página de dados

![](../../../../../.gitbook/assets/image%20%2880%29.png)

### Título

### Nome

### Banco de dados

### Provider

### Tabela

### Índice básico

### Rota

### Permitir Inclusão

### Permitir Edição

### Permitir Exclusão

### Habilita auto-inserção

### Habilita auto-edição

### Permite Visualização

### Exigir Autenticação

### Permitir acesso direto pela URL

### Abre em modo de edição

### Mobile

### Layout responsivo

## Definição de campos da tabela

![](../../../../../.gitbook/assets/image%20%2881%29.png)

### Utilizar todos os campos \(SELECT \* \)

Por padrão, o campo "Utilizar todos os campos \(SELECT \* \), vem selecionado. Isso significa, que todos os campos da tabela definida para o módulo de página de dados serão usados na consulta ao banco de dados. Isso irá ocorrer, independente do campo ser efetivamente usado ou não dentro do módulo.

Na lista de campos que é mostrada acima, existem todos os campos da tabela e na frente uma caixa de seleção para marcar ou não o uso do campo.

Caso não tenha intenção de usar o campo da tabela dentro do módulo, seja em controles ou qualquer outra referência, desmarque o campo correspondente. Isso fará com que o tráfego de dados necessários para alimentar o conteúdo da página seja o mínimo necessário, otimizando a velocidade de carga do módulo.

{% hint style="info" %}
Especialmente as tabelas que possuem muitos campos e registros, lembre de selecionar os campos usados no módulo específico de página de dados. Essa á uma prática importante para melhoria do desempenho da carga do módulo.
{% endhint %}

{% hint style="warning" %}
Caso venha a ter necessidade de editar o módulo e não encontre nas propriedades dos controles ou fórmulas os campos necessários, lembre-se de revisar essa definição para que os campos se tornem disponíveis.
{% endhint %}

### Descrição

Campo livre que poderá usar como documentação do módulo a fim de orientação sobre o objetivo, o conteúdo, as regras, que sirvam de orientação para a equipe de desenvolvimento ou facilite o entendimento do mesmo em outras épocas em que o módulo seja trabalhado.

