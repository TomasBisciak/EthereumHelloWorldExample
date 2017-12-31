# EthereumHelloWorldExample
Example of Hello world written in solidity.

What you will need to run this example:

ethereumjs-testrpc  =   npm install -g ethereumjs-testrpc
truffle             =   npm install -g truffle
ganache-cli         =   npm install -g ganache-cli

Run server with - ganache-cli -i 1001
Where -i specifies the ID for network.
I used 1001 , you can change this , bud then you will have to change truffle-config.js :) with proper ID. or use * for any

Then to compile and run your code use commands :
truffle compile
truffle migrate

To test your method go to console:
truffle console

And to invoke your method use js:
var hw=HelloWorld.at(HelloWorld.address);
hw.sayHello.call()


And you should see 'Hello 2018!'
