---
description: >-
  A aba Provider dá acesso ao editor de código C# para edição específica da
  classe de acesso a dados do módulo que se está trabalhando.
---

# Provider

![](../../../.gitbook/assets/image%20%2885%29.png)

Disponível nos módulos com acesso a dados, a aba Provider, semelhante a aba C\#, é um editor de código C\# que edita diretamente a classe de Provider do módulo em edição. A classe de Provider é responsável pelas operações no banco de dados, inclusive de processos e lançamentos.

Ao abrir a aba Provider, sem que tenha acrescentado nenhuma codificação, vê-se que estamos editando uma classe parcial \(partial class\). Isso significa que outra parte da edição da referida classe está sendo feita em outro arquivo. Dessa forma, seguindo o conceito de classes parciais do .NET Framework, toda a codificação necessária para as operações nativas do banco de dados já estão editadas pelo Gvinci e o que se propicia com a aba Provider é uma extensão das implementações nativas, podendo adicionar ao provider do módulo, os métodos e propriedades que achar adequado aos requisitos de projeto.

As implementações de código que tenham como objetivo a definição de regras de negócios que envolvam acesso a dados devem ser realizadas nessa aba.

As classes parciais de provider no Gvinci, herdam as definições da GeneralProvider.cs que fica gravada na pasta App\_Code\Base.

Na aba "Definitions", se define um nome de Provider. Assim, nas páginas de dados, por exemplo, o nome definido será acrescido do sufixo PageProvider para definição do nome da classe que será gerada em App\_Code\PageProviders.

![](../../../.gitbook/assets/image%20%2883%29.png)

Veja abaixo a definição da classe usando o nome de Provider definido no projeto, acrescido do sufixo PageProvider.

![](../../../.gitbook/assets/image%20%2884%29.png)

Observe agora, no projeto aberto no Visual Studio, como o método editado na aba Provider é acrescentado a classe CadastroClientesPageProvider que já tem toda a implementação nativa criada pelo Gvinci.

![](../../../.gitbook/assets/image%20%2882%29.png)

{% hint style="info" %}
Normalmente não é necessária implementação manual para se realizar todas as operações padrão de CRUD ou processos/lançamentos.
{% endhint %}

{% hint style="warning" %}
 Tenha como regra que as classes de acesso a dados nativas do Gvinci já estão com as devidas restrições de acesso.
{% endhint %}

{% hint style="success" %}
É seguro que implementações extras relacionadas com as operações de banco de dados sejam realizadas por meio da aba Provider, mesmo que seja possível também se realizar essas mesmas operações por meio de código na aba C\#
{% endhint %}

