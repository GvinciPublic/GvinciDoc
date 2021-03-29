# Variáveis de ambiente

Variável de ambiente é uma variável que contém informações sobre o sistema operacional, caminhos de diretórios e as preferências do usuário.

Uma variável de ambiente possui valor dinâmico, que é carregado na memória, e pode ser utilizado por vários processos que funcionam ao mesmo tempo.

Esse tipo de variável se mantém com o mesmo valor para toda uma sessão de uma página ou seja, se você fez o login no site, seu login se mantém para a mesma sessão. Toda página acessada verificará se sua sessão está autenticada, contendo o tempo de duração da sessão que termina automaticamente.

O término da sessão provoca a expiração de uma sessão e com isso, as variáveis de ambiente armazenam valores que se mantêm enquanto essa sessão estiver ativa.

As variáveis de ambiente também são chamadas de variáveis de sessão.

São exemplos de variáveis de ambiente:

• Nome do computador;  
• Data atual;  
• Hora atual;  
• Unidade de disco utilizada no momento;  
• Caminho do diretório que está sendo usado.  
  
No **Gvinci,** as variáveis de ambiente são usadas em processos, lançamentos e fórmulas. A lista segue abaixo:  
• Login do usuário logado;  
• Usuário logado;  
• Nome do desenvolvedor \(projetista\);  
• Observação do usuário logado;  
• Grupo logado;  
• Id do Grupo logado;  
• Versão do projeto;  
• Título do módulo;  
• Título da solução;  
• Título do projeto.

