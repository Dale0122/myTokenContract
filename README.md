# Hello World

Hello! This Solidity program is a simple contract that demonstrates a basic minting and burning functionality using the Solidity programming language. The purpose of this program is to show what I have learned from Metacrafters.io and is made to submit as a project.

## Description

This program shows a simple contract written in Solidity, a programming language that is used for developing smart contracts on the Etherium blockchain. It's easy to use and fun! The contract has a few variables declared for storing the token name, token abbreviation, and the total supply. It also has a mapping variable which maps an address with a uint which is a balance of the user. The contract has 2 functionalities which are "mint" for adding value in the balance and "burn" for subtracting value in the balance as well. This contract paves the way to getting better in programming in Solidity.

## Getting Started

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., myToken.sol). Copy and paste the following code into the file:

```javascript
contract MyToken {

    string public tokenName = "META";
    string public tokenAbbrv = "MTA";
    uint public totalSupply = 0;

    mapping(address => uint) public balances;

    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }

    function burn (address _address, uint _value) public {
        if (balances[_address] >= _value) {
            totalSupply -= _value;
            balances[_address] -= _value;
        }
    }
}

```

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4" (or another compatible version), and then click on the "Compile myToken.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the mint and burn function. Click on the "balances" function to retrieve the balance of the address. Finally, click on the "tokenAbbrv" button to execute the function and retrieve the Token Abbreviation, "tokenName" button to execute the function and retrieve the token name, and lastly "totalSupply" to execute and retrieve the total supply of the account.

## Authors

Francis Dale P. Cañon
[@diejobuuu](https://facebook.com/diejobuuu)


## License

This project is licensed under the MIT License.
