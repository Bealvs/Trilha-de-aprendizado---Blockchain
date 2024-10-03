# Bitcoin e Blockchain - Conceitos Fundamentais

De forma resumida, consiste em mostrar e ensinar como é o funcionamento e conceitos básicos com relação ao Bitcoin, Blockchain e Ethereum. 

## Bitcoin

O bitcoin surgiu durante o contexto de crises e revoltas da Crise econômica de 2008 com planos bilionários de resgate a bancos, muitas vezes sem contrapartida para a população afetada.

Sobre as principais funções que o bitcoin agrega, têm-se:

-  Moeda de troca (Unidade de troca);
-  Reserva de valor;
-  Meio de pagamentos (Sistema de pagamentos).

É importante ter em mente que ele funciona graças a combinação de criptografia, blockchain, descentralização das redes e engenharia de incentivo. Além disso, existem diversas coisas que o sistema financeiro provê que o bitcoin *ainda* não consegue.

Observe a seguinte tabela:

||Bitcoin|Bancos|
|-|-|-|
|Contabilidade|Blockchain|Centralizada|
|Armazenamento|100%|Fracionado|
|Segurança|Criptográfica|Institucional|
|Emissão de moeda|Algoritmo|Política econômica|
|Transações|Distribuído|Centralizado|
|Autenticação|Blockchain|Baseado em sistemas de identificação|
|Regulamentação|Ainda indefinido|Banco Central, normas|
|Processo de decisão|Consenso|Arbritário|
|Controle do dinheiro|Você|Banco|

## Blockchain

### Conceitos básicos

É uma estrutura para armazenamento de dados que consiste em uma cadeia de blocos interconectados e cada bloco contém informações que apontam para o anterior, o que garante a integridade da cadeia para evitar que ela quebre. Além disso, também há a função hash que transforma os inputs, de qualquer tamanho, em um output aparentemente aleatório, com tamanho fixo. São caracterizadas por serem fáceis de computar (criptográficas), unidirecionais, livres de colisão e puzzle friendly (pois caso haja a necessidade de encontrar um hash, mesmo que o conteúdo seja semelhante, ele será diferente).

### Assinaturas digitais

Sobre as assinaturas digitais, são formas de autenticação dos documentos, já que por exemplo, caso seja feita alguma transação, é necessário que ela contenha uma assinatura. Ela é caracterizada por só um indivíduo ser capaz de assinar (de usá-la), ser única para cada documento, qualquer um poder ver que é sua no sentido que é fácil fazer a verificação. É importante destacar que cada chave pública é atrelada a uma chave secreta, esta última não pode ser vazada, pois permite a geração de assinaturas digitais. A chave pública é importante para que qualquer um possa verificar se a assinatura digital em determinado documento é autêntica. É interessante fazer mais de um par de chaves públicas/privadas no caso de roubo, assim o indivíduo não seria totalmente roubado.

### Criando uma Moeda Virtual 

A moeda CentralCoin foi usada para explicar o funcionamento das moedas virtuais, em específico o bitcoin. A única diferença é que na CentralCoin existe uma autoridade central que verifica as transações e mantém a blockchain, enquanto no Bitcoin isto é feito em uma rede descentralizada. São armazenadas as transações de criação e de transferência de moedas CentralCoins na sua blockchain. E para fazer as transações o usuário deve indicar quais moedas está utilizando, nesse caso que ele vai destruir, quais os destinatários das novas moedas que vão ser criadas e adicionar a sua assinatura digital no processo. É importante lembrar que a soma das moedas que vão ser destruídas deve ser maior que as que vão ser criadas, pois há uma taxa.

### O bitcoin

Sobre a rede bitcoin, ela deve ser distribuída, sem hierarquia e seguir um protocolo de consenso. Há nós ao longo da rede, que representam qualquer computador conectado a ela. Existem *full nodes* e *lite nodes*, basicamente o primeiro, em geral, armazena toda a blockchain e é capaz de operar independentemente. Enquanto o segundo, seria inclusive, mais voltado para dispositivos com pouca memória. Foi mencionado o protocolo da fofoca como sendo um nó repassando aos demais que havia recebido transações.

### Proof of Work

Basicamente, o nonce é um valor numérico sem significado que é adicionado a cada bloco da blockchain. Os mineradores alteram o valor do nonce tentando cumprir com o requisito do proof of work que é o mecanismo de consenso utilizado pela rede Bitcoin para validar transações. 

Para o minerador colocar o próximo bloco precisa conseguir criar um bloco cujo hash tenha um determinado número de zeros, que seria chamado de dificuldade. Depois ele avisa aos demais, e todos deveem aprovar. Caso dois mineradores encontrem o bloco ao mesmo tempo, ganha quem tiver mais blocos subsequentes. 

*Mining pools* são esquemas entre mineradores, em que todos trabalham minerando e os Bitcoins conquistados são distribuídos entre todos os participantes de acordo com o trabalho computacional de cada um.  
 
O saldo em bitcoins é a soma de todas as moedas (ainda não destruídas para fazer transações) que foram criadas e destinadas às chaves públicas que o indivíduo em questão controla.

## Carteiras

As principais características delas são:  
- Conveniência;
  - Facilidade e praticidade de uso. 
- Disponibilidade;
  - Usar em qualquer momento.
- Segurança. 
  -  Difícil de roubar.

### Tipos carteiras

De papel:
- Estão escritas uma chave pública e uma privada correspondente;
- É segura dependendo de como é guardada, depende do indivíduo;
- Imune a hackers, enquanto os procedimentos estiverem relacionados ao papel e não ao computador;

De hardware:
- Muito seguras, até com o computador infectado;
- Armazena as chaves secretas e realiza as transações pelo próprio hardware;
- É cara;
- Recuperação de dados é possível.

De Software:
- Múltiplos pares de chaves;
- Recuperação de dados;
- Tão segura quanto for o computador.

Online:
- Arriscada, mas prática;
- Não se sabe qual é a chave secreta.

## Exchanges

São sites que conectam pessoas interessadas em comprar com pessoas interessadas em vender Bitcoin, cobrando uma pequena taxa para isso. São semelhantes às bolsas de valores. É importante destacar que os bancos são regulados, elas ainda não são, o que as tornam arriscadas e alvos de hackers com frequência.

Elas não tem:
- Requerimentos de reserva;
- Controle de investimentos;
- Fundo garantidor de créditos;
- njeções de liquidez.

## Anonimato 

Quando se trata de fazer transações e doações, têm-se o devate sobre ser ou não anônimo. E tecnicamente não é, por serem rastreáveis. Não é o ideal que alguém consiga associar a identidade de algum indivíduo com a chave 
pública dele, pois haveria como saber o que ele faz, o que compra, com que frequência faz determinadas compras...

## Conteúdo extra
### Ethereum

- Comunidade ativa;
- Conceitualmente diferente do bitcoin por ser possível executar programas na rede;
- É possível ter várias contas;
- Smart contracts;
- Moeda Ether;
- Mineração Memory Hard;
- Consenso guiado;
- Descentralizada.

