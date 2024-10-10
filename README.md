# Atividade individual - Implementação da Blockchain 
O objetivo da atividade é desenvolver uma "rede blockchain" com funcionalidades básicas. O projeto foi desenvolvido em Javascript e consiste numa blockchain simples que permite a criação de transações, que são colocadas nos blocos e estes são colocados na rede. Trata-se de uma atividade individual proposta durante o programa de bolsas de Blockchain da empresa Compass UOL.

---

## É necessário ter: 

:triangular_flag_on_post: [Node.js](https://nodejs.org/en/download/package-manager/current)

---

## Passo-a-passo:

- Primeiro deve-se dar `git clone` e copiar o link que aparece após clicar em [*Code <>*](https://github.com/Bealvs/Trilha-de-aprendizado---Blockchain.git)
- Ao clonar o repositório, abra o terminal e digite `npm install`
- Exitem duas bibliotecas que serão instaladas:
  - crypto-js
  - date-fns
- Após isso, basta executar o arquivo através do comando: `node .\Atividade.js`
    - OBS.: A fim de facilitar, utilize o comando `node` e aperte *TAB*.

---

## Sobre o código

Existem as seguintes classes:
- :black_square_button: Bloco
  - Apresenta a estrutura básica que é composta por: índice, nonce, hash do bloco, hash do bloco anterior, data de criação e os dados (neste caso o foco seriam as transações, mas também é possível colocar da seguinte forma: `blockchain.mineracao("Informações...");`)
    
- :money_with_wings: Transação
  - É composta pelo remetente, moeda, valor (no sentido de quantidade) e destinatário. Essas informações podem ser inseridas da seguinte forma: `blockchain.mineracao(new Transacao("Geisy", 10, "Bitcoins", "Gabriel"));`. Também podem ser inseridas mais de uma transação: `blockchain.mineracao([new Transacao("Wandreus", 9, "Bitcoins", "Geisy"), new Transacao("Gabriel", 34, "Bitcoins", "Juliana"), new Transacao("Guilherme", 12, "Bitcoins", "Thuli")]);`
    
- :chains: Blockchain (É composta por métodos)
  - Seus métodos são voltados para: fazer o bloco Genesis, verificar o último bloco, minerar, validar o hash e validar bloco por bloco.  

Caso surja alguma dúvida, por favor submeta uma nova *Issue*.
