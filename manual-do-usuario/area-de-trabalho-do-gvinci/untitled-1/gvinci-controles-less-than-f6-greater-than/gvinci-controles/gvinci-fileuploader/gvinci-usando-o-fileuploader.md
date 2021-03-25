# Gvinci : Usando o FileUploader

O controle **FileUploader** é utilizado para fazer download e upload de arquivos.

![](http://www.gvinci.com.br/manual/fileupload1.zoom71.png)

Na propriedade **AllowFileExtensions** você pode determinar quais as extensões de arquivos que serão aceitas para upload.

![](http://www.gvinci.com.br/manual/allowfileextensions.png)

O botão ![](http://www.gvinci.com.br/manual/abrirfu.png) é usado para listar arquivos que podem ser carregados \(upload\). Os arquivos escolhidos na caixa **Abrir** devem possuir as extensões permitidas na propriedade **AllowFileExtensions.**

Na seção "Arquivo" irá aparecer o nome do arquivo para fazer upload. Para fazer o download do arquivo, basta clicar sobre o nome do arquivo e determinar um local para o armazenamento.

![](http://www.gvinci.com.br/manual/nomearquivofu.png)

Ao carregar um arquivo grande, um vídeo \*.avi por exemplo, o controle exibe uma barra de progresso com o carregamento do arquivo e a opção para cancelar o upload.

![](http://www.gvinci.com.br/manual/fuloading.png)

Após clicar em ![](http://www.gvinci.com.br/manual/cancelfu.png), aparece a opção para remover o arquivo da lista de upload.

![](http://www.gvinci.com.br/manual/removefu.png)

A propriedade **MaxFileSize** define o tamanho máximo do arquivo para upload em Bytes.

![](http://www.gvinci.com.br/manual/maxfilesize.png)

Caso o arquivo para upload não esteja de acordo com os valores das propriedades **MaxFileSize** e **AllowFileExtensions,** ou seja, não esteja com o tamanho permitido e com extensão permitida, a seguinte mensagem será exibida:

![](http://www.gvinci.com.br/manual/arquivoinvalidofu.zoom93.png)

Na propriedade **ShowPreview** podemos ativar a exibição do conteúdo do arquivo:

![](http://www.gvinci.com.br/manual/showpreviewfu.png)

O conteúdo do arquivo será exibido, caso o valor da propriedade seja True e o arquivo seja do tipo imagem.

![](http://www.gvinci.com.br/manual/beachfu.png)

A propriedade **SaveAsFile** permite que o arquivo para download seja armazenado em uma determinada pasta. Ao colocar o valor **"True"** nesta propriedade, a propriedade **Path** é exibida, solicitando o caminho para o armazenamento do arquivo.

![](http://www.gvinci.com.br/manual/saveasfile.png)

