# Hello World

Hello! This Solidity program is a simple contract that demonstrates a basic minting and burning functionality using the Solidity programming language. The purpose of this program is to show what I have learned from Metacrafters.io and is made to submit as a project.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a single function that returns the string "Hello World!". This program serves as a simple and straightforward introduction to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

This program shows a simple contract written in Solidity, a programming language that is used for developing smart contracts on the Etherium blockchain. It's easy to use and fun! The contract has a few variables declared for storing the token name, token abbreviation, and the total supply. It also has a mapping variable which maps an address with a uint which is a balance of the user. The contract has 2 functionalities which are "mint" for adding value in the balance and "burn" for subtracting value in the balance as well. 

## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

```javascript
pragma solidity ^0.8.4;

contract HelloWorld {
    function sayHello() public pure returns (string memory) {
        return "Hello World!";
    }
}

```

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4" (or another compatible version), and then click on the "Compile HelloWorld.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "HelloWorld" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the sayHello function. Click on the "HelloWorld" contract in the left-hand sidebar, and then click on the "sayHello" function. Finally, click on the "transact" button to execute the function and retrieve the "Hello World!" message.

## Authors

Francis Dale P. Cañon
[@diejobuuu](https://facebook.com/diejobuuu)


## License

This project is licensed under the MIT License.
