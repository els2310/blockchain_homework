# Vemmi Network documentation 
---
## Environments and dependencies
We installed "Go Ethereum Tools" including the Geth & Tools features. <br />
[Go Ethereum Tools](https://geth.ethereum.org/downloads/) 

Here is the file for the JSON conde with the Vemmi Network configuration <br />
[Vemmi Network JSON](../blockchain_homework/VemmiChain/vemmi.json) 

## Geth flags
We need to initialize each node with the Vemmi Network. 
- Node 1: `./geth --datadir node1 init vemmi.json`
- Node 2: `./geth --datadir node2 init vemmi.json`

We need to run each node in separate terminal windows with the commands:
- Node 1: `./geth --datadir node1 --unlock "0x5d129322100c469011cd4b2Db8Da14E3b435Ff61" --mine --rpc --allow-insecure-unlock`
- Node 2: `./geth --datadir node2 --unlock "0x4f7082f3907f5eEc087b469d36427a7637859869" --mine --port 30304 --bootnodes "enode://211d10ac0643f1386b98fd60a7bf8d0e213eac8506dbb61ea5a8efbd8598d38e6f143a77649f1cf6773d3f8d1fdbb709c837f705c28df0fcb94d7cdadc087d88@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock`


## Network configuration 
![Network configuration ](../Screenshots/terminal_POA_conf.png) 


##### Node 1
- Chain ID: 1430 
- Account password: 14002

##### Node 2
- Chain ID: 1430 
- Account password: 1202

## MyCrypto 
#### Making a transaction
We need to enter node 2 public address and select amount to transafer
![t1](../Screenshots/transaction_1.png) <br />

We confirm the transfer
![t2](../Screenshots/transaction_2.png) <br />

We can see transfer is pending 
![t3](../Screenshots/transaction_3.png) <br />

Now transfer is completed
![t4](../Screenshots/transaction_4.png) <br />

We can notice that the balance has decreased 
![t5](../Screenshots/transaction_5.png) <br />


