# my_blockchain

## Description

my_blockchain is a command that allows for the creation and managment of a blockchain via the command line interface. When the program starts, a prompt appears. If there is a previously generated blockchain file in the root directory, it will automatically upload and begin with the saved blockchain. The prompt allows the user to enter commands the following commands for execution: 



Valid expressions:
- ```add node nid``` add a nid identifier to the blockchain node
- ```rm node nid...``` remove nodes from the blockchain with a nid identifer. If nid is '*' then all nodes are impacted
- ```add block bid nid...``` add a bid identifier block to nodes identified by nid. If nid is '*', then all nodes are impacted
- ```rm block bid...``` removed the bid identified blocks from all nodes where these blocks are present
- ```ls``` list all nodes by their identifiers. The option -l attaches the blocks bid's associated with each node
- ```sync``` synchronize all of the nodes with each other. Upon issuing this command, all of the nodes are composed of the same blocks
- ```quit``` save and leave the blockchain

The blockchain prompt displays:
```
a [ character
a first letter that indicates the state of synchronization of the chain:
"s" if the blockchain is synchronized
"-" if the blockchain is not synchronized.
n number of nodes in the chain.
the "]> " string (with a space)'
```

## Error Messages
```
1: no more resources available on the computer
2: this node already exists
3: this block already exists
4: node doesn't exist
5: block doesn't exist
6: command not found
```

## How to compile

Compile by running make in the root directory