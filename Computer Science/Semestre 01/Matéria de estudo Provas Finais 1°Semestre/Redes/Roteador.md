> O que é?
> Um **roteador** é um dispositivo de rede inteligente que direciona pacotes de dados entre diferentes redes. Ele opera na **Camada 3 (Camada de Rede)** do Modelo OSI.

#### Características do Roteador:
- **Direcionamento de Dados:** 
	Roteadores usam endereços IP para encaminhar dados especificamente para o dispositivo de destino, seja dentro da mesma rede ou em uma rede diferente.
- **Segmentação de Rede:** 
	Conecta diferentes redes, como uma LAN doméstica à Internet.
- **Segurança e Filtragem:** 
	Oferece recursos de segurança, como firewalls, NAT (Network Address Translation) e controle de acesso.
- **Gerenciamento de Tráfego:** 
	Gerencia o tráfego de dados para otimizar o desempenho da rede, evitando congestionamento e colisões.
- **Suporte a Protocolos:** 
	Suporta vários protocolos de rede, como TCP/IP, e pode realizar roteamento dinâmico usando protocolos como OSPF (Open Shortest Path First) ou BGP (Border Gateway Protocol).

### Comparação Entre Hub e Roteador

|Característica|Hub|Roteador|
|---|---|---|
|**Camada OSI**|Camada 1 (Física)|Camada 3 (Rede)|
|**Transmissão de Dados**|Repassa dados para todas as portas|Direciona dados para dispositivos específicos|
|**Filtragem de Dados**|Não|Sim|
|**Colisões de Dados**|Alta chance de colisões|Menor chance, pois gerencia tráfego|
|**Segurança**|Básica ou inexistente|Avançada, com firewalls e NAT|
|**Custo**|Geralmente mais barato|Mais caro, mas com mais funcionalidades|
|**Uso Comum**|Pequenas redes locais simples|Conexão de redes diferentes (ex.: LAN à Internet)|
### Exemplo Prático

#### Hub:

Imagine uma pequena rede de escritório com 4 computadores conectados a um hub. Quando o computador A envia dados, o hub envia os dados para os computadores B, C e D, mesmo que o destinatário seja apenas o computador B. Isso pode causar congestionamento e colisões de dados.

#### Roteador:

Agora, imagine uma casa conectada à Internet através de um roteador. O roteador conecta todos os dispositivos (computadores, smartphones, tablets) à Internet e entre si. Quando um dispositivo envia dados, o roteador garante que os dados cheguem ao destino correto, seja outro dispositivo na rede doméstica ou um servidor na Internet.