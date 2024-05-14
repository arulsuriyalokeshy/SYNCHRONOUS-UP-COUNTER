### CREATING A PRIVATE BLOCKCHAIN.


**AIM:**<br>
To create a private blockchain, add nodes and create account to bransfer ethereum into it using geth.

**SOFTWARE REQUIRED:**

Hardware: PC

software: Geth, VS Code, Remix




**PROCEDURE:**
1. Download the geth, software for windows and install it into your computer<br>

2. To check whe ther geth is toistalled or not, run the command. "Geth" in your computer.<br>

3. create a directory name go- ethereum.<br>

4. Then create two nodes within go- ethereum.<br>

named node i and node 2<br>

5. open vs code using the command "Code"<br>

6. create account for two. nodes by using<br>

geth-datadir "/data" account new"<br>

7. Create a genesis block "private block.json" inside go-ethereum<br>

8. Give node address in signel address, ether amount with gas eimit.<br>

9. To configure both nodes using genesis block. run "geth Json. datadir. I data init -- / private block.<br>

10. Create a bootnode and generate a bootkey

bootnode- genkey boot.Key.

→ bootnode - nodekey boot key verbority T-adda "127.0.0.1:30301"<br>

11. Run two nodes<br>

12. Create password .txt under both nodes and save Password in it.<br>

13. Get into Remix and change the environment into custom external HTTP provider<br>

14. Create a new contract named New. sol.<br>

15. save it and click deploy.<br>








**PROGRAM**<br>
```
{

Config"

"Chain Id: 878787,

"homestead Block":0,

"eip 150 block": 0,

"eip 155 block":0,
10 eip 158 block": 0,

"byzantium block": 0,

"peters burgblock":0ишния си хо

"berlin block": 0,

" unique": {

"period": 5,

"epoch": 30000.

}

},

"difficulty": "1";

"gaslimit": "8000000",

"extradata": "0x0. {Signer addressfo...",

"alloc": {

"nodel addr": {"balance" : "ether"},

"nodez addr": {"balance": "ether"},



// Solidity program

//SPDX-License Identifier: MIT

pragma solidity 0.8-19:

Contract New &

Stung name;

function setName (string memory-name) publict

name = name;

}



```
DEPLOY AND RUNNING TRANSACTIONS
IN REMIX.
![WhatsApp Image 2024-05-06 at 18 11 55_9d772bac](https://github.com/arulsuriyalokeshy/SYNCHRONOUS-UP-COUNTER/assets/149130151/5c28e1d7-ef16-438a-acad-6e3ef88a41ee)

* By using solidity program, New sol the new Contract is created and the ethereum is transferred.


**OUTPUT**<br>
RUNNING BLOCK CHAIN.<br>
![WhatsApp Image 2024-05-06 at 18 11 55_e7d50cb5](https://github.com/arulsuriyalokeshy/SYNCHRONOUS-UP-COUNTER/assets/149130151/a8a9247b-57ef-46ad-8f01-7c385d2033a0)
<br>


The first block is added using geth and deploying using Remix<br>


**RESULTS**<br>
Thus the private Block is build and ethereum is transferred successfully using geth.
