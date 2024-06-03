#### Estrutura
- **Formato:** IPv6 utiliza um formato de 128 bits, representado por oito grupos de quatro dígitos hexadecimais separados por dois pontos (por exemplo, 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
- **Exemplo:** 2001:0db8:85a3:0000:0000:8a2e:0370:7334

#### Características
- **Capacidade:** 
	Suporta aproximadamente 340 undecilhões de endereços (2^128 endereços), o que resolve o problema de esgotamento de endereços do IPv4.
- **Notação Hexadecimal:** 
	Usa dígitos hexadecimais (0-9 e a-f) para representar os 128 bits.
- **Abreviação:** 
	Pode ser abreviado omitindo zeros à esquerda em cada grupo e substituindo sequências contínuas de zeros por "::" (por exemplo, 2001:0db8::8a2e:0370:7334).

#### Benefícios
- **Espaço de Endereçamento Expandido:** 
	Permite um número praticamente infinito de endereços únicos.
- **Melhoria na Configuração:** 
	Suporte para autoconfiguração de endereços, facilitando a configuração de dispositivos na rede.
- **Segurança Integrada:** 
	Suporte nativo para IPsec (segurança no nível de IP).

### Comparação entre IPv4 e IPv6

|Característica|IPv4|IPv6|
|---|---|---|
|**Formato**|32 bits, decimal (ex.: 192.168.1.1)|128 bits, hexadecimal (ex.: 2001:db8::1)|
|**Capacidade de Endereço**|4,3 bilhões de endereços|340 undecilhões de endereços|
|**Configuração**|Manual ou DHCP|Autoconfiguração, DHCPv6|
|**Segurança**|Opcional (IPsec)|Obrigatório (IPsec nativo)|
|**Roteamento**|Mais complexo, com NAT|Roteamento mais simples, sem necessidade de NAT|