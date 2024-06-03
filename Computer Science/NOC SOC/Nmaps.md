> Conhecimento é poder, quanto mais conhecimento sobre um sistema ou network alvos, maior é o nosso leque de opções. É por isso que uma *enumeração apropriada exista antes de qualquer tentativa de exploit.*

> [!NOTE] Por Exemplo:
> Antes de performar uma audição de de segurança em um dado endereçamento de IP (ou multiplos), *é necessário mapear quais serviços estão sendo rodados pelo target* (um webserver, ou um windows active directory domain controller). 

# Ports

> ***Conexões de rede são feitas entre dois ports** (ou duas portas de rede), uma porta aberta recebendo no servidor, e uma porta* aleatóriamente *selecionada na sua máquina.*

> O primeiro passo seria realizar algo conhecido como **port scanning**. Quando um computador roda qualquer serviço de network, ele abre um network port para receber a conexão. **Ports são necessários para fazer multiplos requests de rede ou ter mais serviços disponíveis.** 


>[!NOTE] Por Exemplo:
>Ao abrir várias páginas em um único browser, o programa deve ter uma forma de determinar que aba está carregando que página. Isso é feito estabelecendo **conexões com o servidor web usando ports diferentes na sua máquina local.** 
>Igualmente, se o objetivo for com que um servidor rode mais de um serviço (duas versões de um site: HTTP e HTTPS) **então é preciso de uma forma de direcionar o tráfego para o serviço apropriado**, ports são a solução para isso.


>[!NOTE] Exemplo:
>Ao se conectar com uma página web, seu computador pode abrir uma nova porta**(49534)** para se conectar com a **porta 443** de um servidor.
 
![[3XAfRpI.png]]




