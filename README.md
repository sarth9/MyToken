# MyToken Smart Contract
A simple Solidity smart contract for creating and managing a custom ERC20-like token with basic minting and burning functionalities.

## Description
The MyToken contract allows you to create a token with a specific name, abbreviation, and total supply. Users can mint new tokens to increase the total supply and burn tokens to reduce the total supply. The contract includes safety checks to ensure that only valid operations are executed.

## Getting Started
### Installing
1. Clone the Repository:
```
git clone https://github.com/DipeshChadha/EthProject.git
cd mytoken
```

2. Open in Your IDE:
Open the cloned repository in your preferred Integrated Development Environment (IDE) that supports Solidity, such as Remix.

3. Install Dependencies:
If you are using a local development environment, make sure to install all necessary dependencies for Solidity development, such as Solidity compiler.

### Executing Program
To deploy and interact with the contract, follow these steps:

1. Compile the Contract:
Open the MyToken.sol file in Remix or your IDE, and compile it to check for any errors.

2. Deploy the Contract:
In Remix, choose the appropriate environment and click on the "Deploy" button.

3. Interact with the Contract:

Mint Tokens:
Use the mint function to increase the supply of tokens.
```
// Example to mint 100 tokens to the specified address
myToken.mint("0xYourAddressHere", 100);
```
Burn Tokens:
Use the burn function to reduce the supply of tokens.
```
// Example to burn 50 tokens from the specified address
myToken.burn("0xYourAddressHere", 50);
```

4. Verify Balances:
You can check the balance of any address using the balances mapping.
```
// Example to check the balance of an address
uint balance = myToken.balances("0xYourAddressHere");
```

## Help
Common issues and solutions:

* Insufficient Balance for Burning:
The burn function checks if the address has sufficient balance before proceeding. Ensure that the address has enough tokens to burn.
```
// Command to view more details
myToken.balances("0xYourAddressHere");
```

## Authors
Sarth
* GitHub: @sarth9
* Email: sarth0903@gmail.com
