>	 Sistema de [[Base 2]] constituído pelos dígitos 0 e 1
>	 É o sistema utilizado por computadores para comunicacao entre software e hardware.
>	 A criacao do Sistema Binário pode ser atribuída ao matemático [[Leibniz]]

### Transformando Sistema binário para Sistema Decimal
Para realizar a **conversão** de **[[Sistema Decimal]] para binário**, realiza-se a divisão sucessiva por 2
A leitura do resultado é feita do último quociente para o primeiro resto.
Para se converter um número de binário para decimal, deve-se multiplicar cada bit pela potência de sua posição e somar os resultados.

Por exemplo, a conversão do número 1011(base2)  para decimal é feita da seguinte forma:

|                      |                        |         |         |         |
| -------------------- | ---------------------- | ------- | ------- | ------- |
| **Binário**          | 1                      | 0       | 1       | 1       |
| **Valor da posição** | 1 X 2^3                | 0 X 2^2 | 1 X 2^1 | 1 X 2^0 |
| __                   | 8                      | 0       | 2       | 1       |
| **Resultado**        | 8+0+2 + 1 = 11 decimal |         |         |         |
