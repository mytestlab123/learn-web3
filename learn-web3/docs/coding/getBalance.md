---
sidebar_position: 5
---

# Run first web3 program

### Create app.js with following code

```js
const Web3 = require('web3')
const rpcURL = 'https://rpc.ankr.com/eth'
// const rpcURL = 'https://mainnet.infura.io/v3/' // Your RCkP URL goes here
const web3 = new Web3(rpcURL)
const address = '0x22dA1eEdeBC60C1b8c3a0c48f5C81BBE2b943dD9' // Your account address goes here
web3.eth.getBalance(address).then(console.log);
```

### Run above getBalance function using node

```
node app.js
```