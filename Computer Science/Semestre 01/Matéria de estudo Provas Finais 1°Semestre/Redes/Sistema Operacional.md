# Definição:
 É o **software** fundamental que **gerencia o hardware do computador e os recursos de software**, fornecendo serviços essenciais para os programas de aplicação. Ele atua como uma **interface entre o usuário e o hardware** do computador.
### Gerenciamentos:
##### Processos:
>Criação, escalonamento e término de processos. **O sistema operacional garante que os processos não interfiram uns nos outros.** E gerencia o **uso da CPU.**
##### Memória:
>Controle do uso da memória principal. O sistema operacional aloca e desaloca espaço de memória conforme necessário para diferentes processos.
##### Dispositivos:
>Controle dos dispositivos de entrada e saída conectados ao computador. Ele também **coordena a transferência de dados** entre o computador e esses dispositivos.
##### Arquivos:
>Organização, armazenamento, recuperação, nomeação, compartilhamento e proteção dos **arquivos no sistema de armazenamento**.
##### Segurança e Controle de Acesso:
>Proteção contra **acesso não autorizado aos dados** e recursos do sistema. **Implementa autenticação**, autorização e auditoria.
##### Interface de Usuário:
>Fornecimento de uma interface para que os **usuários interajam com o sistema.** Pode ser uma interface de linha de comando **(CLI)** ou uma interface gráfica do usuário **(GUI).**
   
---
# Kernel:
### Descrição:
   O **kernel** é o **núcleo do sistema operacional**, responsável pela execução e controle das funções mais básicas, como gerenciamento de memória, processos e dispositivos. Ele opera no nível mais baixo de controle do software, **interagindo diretamente com o hardware.**
   
---
# Multiprogramação e Multitarefa:
### Multiprogramação: 
>Multiprogramação é uma técnica utilizada pelos sistemas operacionais para **melhorar a utilização da CPU.** Em um sistema multiprogramado, **várias tarefas (programas) são mantidas na memória ao mesmo tempo.** O sistema operacional **alterna entre essas tarefas,** maximizando o uso da CPU e diminuindo o tempo ocioso.

### Multitarefa:
>Multitarefa refere-se à capacidade de um sistema operacional de e**xecutar múltiplas tarefas ou processos aparentemente ao mesmo tempo.**

>[!NOTE] Tipos de Multitarefa: 
> 
>**Multitarefa Cooperativa:** Os processos voluntariamente cedem o controle da CPU para outros processos. Aqui, o sistema operacional não força a alternância entre os processos; os processos devem ceder o controle voluntariamente.    
>
>**Multitarefa Preemptiva:** O sistema operacional decide quando um processo deve ceder a CPU para outro processo, interrompendo-o temporariamente e alternando para outro processo. Isso permite uma alternância mais eficiente e rápida entre os processos.

#### Como Funciona:
- **Time-Slicing (Fatia de Tempo):** A CPU é dividida em intervalos de tempo e cada processo é executado durante um pequeno intervalo antes de alternar para o próximo processo. Esse processo é conhecido como "time-slicing".
- **Escalonamento:** O sistema operacional utiliza algoritmos de escalonamento (como Round-Robin, Prioridade, etc.) para determinar qual processo será executado a seguir.
---

# Processos e Threads:
### Processos:
>[!NOTE] Definição:
   Um processo é uma **instância de um programa em execução.** Quando você executa um programa, o sistema operacional cria um processo para ele. **Cada processo possui seus próprios recursos, como memória, descritores de arquivos, e estado de execução.**
#### Componentes de um Processo:
1. **Código do Programa:** 
	As instruções que o processo deve executar.
2. **Espaço de Endereçamento:** 
	Inclui a memória onde o código do programa, dados e pilha são armazenados.
3. **Recursos do Sistema:** 
	Arquivos abertos, semáforos, e outros recursos que o processo pode usar.
4. **Contexto de Execução:** 
	O estado atual da CPU para o processo, incluindo registros e ponteiros de pilha.

#### Ciclo de Vida de um Processo:
- **Novo:** 
	O processo está sendo criado.
- **Pronto:** 
	O processo está na fila para ser executado pela CPU.
- **Em Execução:** 
	O processo está sendo executado pela CPU.
- **Bloqueado:** 
	O processo está aguardando por um evento (como I/O).
- **Terminado:** 
	O processo terminou sua execução.

---
### Threads:
> [!NOTE] Definição:
> Uma thread (ou linha de execução) é a **menor unidade de processamento que pode ser programada.** Threads **são partes de um processo que podem ser executadas de forma independente.** Um processo pode ter várias threads compartilhando os mesmos recursos.
#### Vantagens das Threads
1. **Compartilhamento de Recursos:** 
	 Threads dentro do mesmo processo compartilham memória e outros recursos, o que permite comunicação mais eficiente.
2. **Melhor Utilização da CPU:** 
	 Threads podem ser executadas em paralelo em sistemas multicore, melhorando o desempenho.
3. **Menor Custo:** 
	 Criar e gerenciar threads é menos custoso em termos de tempo e recursos do que criar e gerenciar processos.

#### Tipos de Threads
1. **Threads de Usuário:** 
	Gerenciadas pelo próprio programa, sem conhecimento do sistema operacional. Geralmente são mais rápidas, mas podem ser menos eficientes se o SO não as gerenciar diretamente.
2. **Threads de Kernel:** 
	Gerenciadas diretamente pelo sistema operacional, o que permite uma melhor utilização de múltiplos núcleos da CPU.
# Tipos de Acesso e Segurança:

---
### Tipos de Acesso em Sistemas Operacionais:
> [!NOTE] **User-based Access Control - UBAC:** 
> Cada usuário tem permissões específicas que determinam quais recursos podem acessar e quais operações podem realizar.

> [!NOTE] **Role-based Access Control - RBAC:**
> As permissões são atribuídas a funções em vez de usuários individuais. Os usuários são então atribuídos a essas funções, como **"Administrador", "Usuário" e "Convidado".**

> [!NOTE] **Discretionary Access Control - DAC:**
> **O proprietário de um recurso decide quem tem acesso** a ele e quais direitos esses usuários têm, o proprietário de um arquivo pode definir uma **lista de controle de acesso** (ACL) que especifica quais usuários ou grupos podem acessar.

> [!NOTE] **Mandatory Access Control - MAC:**
> As **permissões são definidas por uma autoridade central** com base em regras de segurança predeterminadas e não podem ser alteradas pelos usuários. **Utilizado em sistemas governamentais e militares** onde a segurança é crítica.

### Segurança:
#### Autenticação 
**Definição:** 
- O processo de verificar a identidade de um usuário ou sistema através de senhas, biometria, multifator, etc...
#### Autorização
**Definição:** 
- Determina quais recursos e operações o usuário autenticado pode acessar.
#### Auditoria e Log
**Definição:** 
- Registro de eventos significativos, como tentativas de login, acessos a arquivos e alterações de sistema.
#### Criptografia
**Definição:** 
- Processo de converter dados em um formato ilegível para impedir acesso não autorizado.
#### Proteção contra Malware
**Definição:** 
- Ferramentas e técnicas para detectar e remover software malicioso, como vírus, worms e trojans.
---
