### make directory
```sh
mkdir workspace
cd workspace
mkdir firstproject
```
### Create a bare Truffle project with no smart contracts included
```sh
cd firstproject
truffle init
```
### Open project in visual studio code
```sh
code .
```
### Config truffle-config.js
In Network entry:
```js
development: {
      host: "127.0.0.1",     // Localhost (default: none)
      port: 7545,            // Standard Ethereum port (default: none) Point to the Ganache network
      network_id: "*",       // Any network (default: none)
     }
```
### Create a new smart contract in ./contract
### Create deploy script in ./migration
### Compile, deploy and invoke the contract
```sh
truffle compile
truffle migrate
truffle console
truffle(development)> helloworld.deployed().then(function(instance) {return instance.gethelloMessage()})
```
### Questions: 
#### Do we need contract name same with file name?
https://blog.csdn.net/beiniao520/article/details/79582983
#### SPDX license identifier not provided in source file.
https://forum.openzeppelin.com/t/solidity-0-6-8-introduces-spdx-license-identifiers/2859
#### Pay attention to the solidity version when using vs to compile the contract
Can edit the configuration in extension/setting
