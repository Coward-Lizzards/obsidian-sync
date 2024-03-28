File Transfer Protocol → transferência de arquivos entre dois computadores

[[FTP (File Transfer Protocol)]] é um protocolo de rede para a transmissão de arquivos entre computadores. Dentro do conjunto [[TCP IP]] (Transmission Control Protocol/Internet Protocol), ele é um protocolo da camada de aplicação para o download e upload de arquivos em conexões do tipo _Cliente-Servidor_. 

O [[FTP (File Transfer Protocol)]] permite que desenvolvedores de sites promovam mudanças de maneira conveniente e segura, mesmo que você tenha que transferir um grande número de arquivos.

O protocolo FTP permite que usuários autorizados possam fazer download e upload de arquivos de um servidor FTP, um computador que armazena os dados. Dessa forma, o FTP facilita a transferência de informações entre diferentes dispositivos.

>Existem dois canais distintos de comunicação na hora de se estabelecer uma conexão usando o File Transfer Protocol. O primeiro é o canal de comando, que é onde se inicia a instrução e a resposta. O outro é o canal de dados, onde ocorre a distribuição de dados.
>Se quiser baixar ou transferir um arquivo, um usuário terá que usar o protocolo para solicitar a criação de mudanças no servidor. Em troca, o servidor vai garantir esse acesso. Essa seção é conhecida como “modo de conexão ativa”.
>A distribuição no modo ativo pode enfrentar um problema se o firewall estiver protegendo a máquina do usuário. Normalmente, o firewall não permite quaisquer sessões não autorizadas de um elemento externo.
>O modo **passivo** é usado se esse problema ocorrer. Neste modo, o usuário estabelece tanto o canal de comando quanto o de dados. Este modo então pede que o servidor apenas **“escute”** ao invés de tentar criar uma conexão de volta com o usuário.