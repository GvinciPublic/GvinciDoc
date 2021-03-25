# Integridades

A integridade trata do nível de confiança das informações do banco de dados, isto é, a credibilidade das informações armazenadas.

A integridade no Gvinci é gerada diretamente no banco, através de "Foreign Keys" e "Constraints".

Foreign Keys são chaves estrangeiras que colocamos em campos que tenham relacionamento com outro campo com chave primária \(Primary Key\) de outra tabela.

Constraints são restrições. Por exemplo, determinar uma chave primária \(Primary Key\) para um campo que não pode ter seu conteúdo repetido.

Uma integridade referencial é construída em um campo que se relacione com outro campo que seja chave primária em outra tabela.

Uma forma de garantir a integridade de um banco é controlar os lançamentos que são feitos de uma tabela para outra 

No **Gvinci**, você pode criar e definir os campos para lançamentos. Na tela de definição das propriedades da tabela, no painel **Banco de dados,** os nomes dos campos podem ser inseridos, conforme mostra a figura abaixo:

![](http://www.gvinci.com.br/manual/intlancdlangv5.zoom72.png)

Para detalhes sobre o uso dos lançamentos, consulte **Lançamentos.** 

