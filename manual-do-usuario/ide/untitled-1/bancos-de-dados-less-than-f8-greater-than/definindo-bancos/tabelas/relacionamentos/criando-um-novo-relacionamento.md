# Criando um novo relacionamento

Para criar um novo relacionamento, preencha os campos conforme as explicações abaixo:

![](http://www.gvinci.com.br/manual/novarelac2gv5.zoom80.png)

**Tabela estrangeira:** Adicione aqui o nome da tabela estrangeira onde está o campo que receberá o relacionamento.

**Nome:** Insira um nome para o relacionamento. Este nome será utilizado internamente pela aplicação. O nome sugerido pelo **Gvinci** começa com **FK\_** e em seguida o nome da tabela estrangeira. FK significa Foreign Key \(Chave estrangeira\).

**Título:** Insira um título para o relacionamento. Este título vai aparecer na árvore da estrutura do banco de dados. O título sugerido pelo **Gvinci** é composto pelo nome da tabela base e em seguida o nome da tabela estrangeira.

**Cardinalidade:** Defina se o relacionamento será de \(1-1\) ou de  \(1-N\).

**• Relacionamento 1-1:**  
             • Não realiza deleção dos filhos  
             • Deve ser feita na tabela filha  
             • Esse é um tipo de relação somente de integridade garantindo que o registro filho deve ter um registro pai vinculado  
             • Não permite que o registro pai seja deletado se existir um registro filho  
             • Caso o usuário queira deletar o pai ele terá que deletar todos os filhos antes de deletar o pai  
**• Relacionamento 1-N:**  
             • Essa relação deve ser feita na tabela pai  
             • Esse é um tipo de relação somente de integridade garantindo que o registro filho deve ter um registro pai vinculado  
             • Esse tipo de relação 1-n caso o usuário tente deletar o pai o banco deleta automaticamente todos os filhos vinculados  
             • Deve existir um índice pelos campos que compõem a relação na tabela base \(tabela pai\)

**Tipo de relacionamento:**  
              **• Trigger:** Selecione esta opção se o relacionamento for funcionar automaticamente  
              **• Constraint:** Marque esta opção se o relacionamento funcionar diretamente no banco

**Replicação:**  
             **• Exclusão em cascata:** Apaga todos os registros relacionados com o registro que será apagado. Esta opção é habilitada somente quando a cardinalidade for 1-N  
             **• Atualização em cascata:** Atualiza todos os registros relacionados com o registro que será atualizado

**Campo base:** Adicione o campo da tabela básica.  
**Campo estrangeiro:** Adicione o campo da tabela estrangeira.

