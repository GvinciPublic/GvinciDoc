# Campos

Para inserir campos em uma tabela, siga as instruções abaixo:

**1.** Clique duas vezes sobre a palavra **Tabelas.**

**2.** Clique com o botão direito do mouse sobre **“Campos”**, ou utilize o botão ![](http://www.gvinci.com.br/manual/adicionar.png). Observe a figura abaixo:

![](http://www.gvinci.com.br/manual/criacampo1gv5.zoom80.png)

**3.** Clique em **“Novo Campo”.** Preencha as propriedades conforme explicações abaixo:

![](http://www.gvinci.com.br/manual/criacampo2gv5.zoom80.png)

**Nome:** Identifica o campo dentro do banco de dados. O nome do campo pode conter espaços, acentos e outros caracteres, porém, não pode começar com número.

**Apelido:** Insira aqui um apelido para o campo, que poderá ser usado internamente pela aplicação.

**Título:** Insira o título do campo que vai aparecer na árvore do banco de dados.

**Tipo:** Determina de que tipo será o campo. Os tipos disponíveis são:

![](http://www.gvinci.com.br/manual/bd10.png)

**• Caracter:** Para letras, números e símbolos  
**• Numérico:** Somente para números. O tamanho do campo numérico deve ser maior que 0 e menor que 36  
**• Lógico:** Dados do tipo lógico \(true ou false\)  
**• Binário:** Utiliza o formato binário, próprio para arquivos executáveis, figuras, etc  
**• Memo:** Para grande quantidade de text.  
**• Imagem:** Também usado para imagens  
**• Data/Hora:** Usado para datas ou horas  
**• Data:** Dados do tipo data  
**• TimeStamp:** Usado para data e hora em uma operação de INSERT or UPDATE porque são automaticamente definidas a data e a hora da operação mais recente se você não especificar um valor. Para definir a data e a hora atual é necessário atribuir ao campo um valor nulo, marcando a opção **"Permitir nulo"**

Quando um tipo é escolhido, o **Gvinci** sugere um controle para apresentar o campo criado. Por exemplo, se o campo for do tipo **"Caracter",** então o controle sugerido será um TextBox. Se for do tipo **"imagem"**, o controle sugerido será um **"FileUploader".**

**Utilizar campo customizado:** Habilita a lista de campos customizados logo abaixo. Os campos customizados são criados no painel Controles Customizados.

**Tamanho:** Quantidade máxima de dígitos ou caracteres que poderão ser digitados no campo.

**Decimal:** Caso o campo em definição seja do tipo numérico, você poderá especificar uma quantidade de casas decimais a ser considerada para este campo. Se for especificado um número de casas decimais maior do que 0,  já estará calculada a posição da vírgula, no tamanho do campo.

**Permitir Nulo:** Define se o campo permitirá que sejam gravados valores nulos. Como padrão, esta propriedade já vem desmarcada. Com esta opção desmarcada, quando for feita a gravação dos dados na tabela, o campo obrigatoriamente precisará ter conteúdo.

**Sequência:** Se você preferir que o campo seja incrementado automaticamente, a cada registro que é incluído, marque a opção "Sequencial" e o número "1" será inserido automaticamente. Para aceitar esta opção, o campo deverá ser do tipo numérico. É permitido criar somente um campo sequencial para cada tabela.

**Máscara:** Esta opção controla o formato que a sequência dos caracteres do campo vai aparecer para o usuário. Este recurso diminui as margens de erro de digitação dos usuários da aplicação, inserindo os dados na sintaxe esperada.

A máscara padrão já vem definida para o campo numérico. Por exemplo, se você determinar o tamanho do campo numérico para 3, a máscara sugerida será 999. Você pode personalizar o conteúdo deste campo, definindo como prefere a apresentação dos dados do campo, adicionando uma nova máscara.

Os campos do tipo **lógico**, **imagem**, **memo**, **binário** e **TimeStamp** não possuem máscara.

Os caracteres especiais especificados nas máscaras são:

• \(!\) - significa que o caractere que for digitado nesta posição será transformado para maiúsculo, aceitando qualquer tipo de caractere  
• \(A\) - significa que o caractere que for digitado nesta posição só poderá ser alfabético, acentuado ou não, impedindo a inserção de dígitos numéricos  
• \(9\) - significa que somente dígitos numéricos poderão ser digitados no campo em uma determinada posição  
• \(\#\) - funciona de maneira idêntica ao número 9 com a diferença que espaços também poderão ser digitados  
• \(a\) - significa que somente caracteres alfabéticos minúsculos poderão ser digitados nesta posição  
• \(X\) - significa que qualquer caractere poderá ser digitado na posição  
• arroba \(@\) - é usado, na primeira posição da máscara, em conjunto com qualquer um dos acima especificados. Quando este caractere figura na máscara, o caractere seguinte a este servirá para todos os caracteres digitados no campo. Por exemplo: @! \(tudo maiúsculo\), @A \(tudo alfabético\) etc. Combinações podem ser feitas, como por exemplo: @!@A \(tudo o que for digitado no campo só poderá ser em maiúsculas e alfabético\)

**Valor Padrão :** Permite criar um valor default \(padrão\) para o campo. O valor default é registrado no banco de dados e será gravado quando nenhum valor for enviado ao campo. Esta opção é desativada quando se marca a caixa de verificação "Sequencial", já que, neste caso, o conteúdo do campo vai obedecer uma sequência de inserção.

**Descrição:** Digite informações sobre o campo em definição para que sejam utilizadas na documentação da aplicação, que é gerada pelo **Gvinci.**

**Utilizar controle customizado:** Marque esta opção se o controle para o campo já houver sido criado no painel Controles Customizados. Caso a máscara escolhida seja diferente da máscara do controle customizado, aparecerá a mensagem de confirmação para alteração da máscara.

![](http://www.gvinci.com.br/manual/ctrlcust1gv5.zoom100.png)

**Customizar controle de apresentação:** Habilita o Controle de Apresentação, exibindo as propriedades de Aparência, Comportamento, Layout e Miscellaneous. Esta funcionalidade permite configurar o controle correspondente ao campo que está sendo criado. Por exemplo, caso você escolha o tipo **Lógico** para o campo, o controle customizado sugerido será um **Checkbox.**

![](http://www.gvinci.com.br/manual/custctrlgv5.zoom100.png)

Para mais detalhes, consulte o tópico Controle de apresentação.

