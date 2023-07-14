# YERS Token Contract

This Solidity smart contract represents the YERS token, which allows for minting and burning of tokens. The contract includes the necessary functions to manage the token supply and individual balances.

## Requirements

1. Public Variables:
   - `tokenName`: The name of the token ("YERS").
   - `tokenAbbrv`: The abbreviation or symbol of the token ("YS").
   - `totalSupply`: The total supply of the YERS tokens.

2. Mapping:
   - `balances`: A mapping of addresses to their corresponding token balances.

3. Mint Function:
   - `mint(address _address, uint _value)`: Increases the total supply of tokens by the given value and increases the balance of the specified address by that amount.

4. Burn Function:
   - `burn(address _address, uint _value)`: Decreases the total supply of tokens by the given value and decreases the balance of the specified address by that amount. It only burns tokens if the balance of the address is greater than or equal to the amount to be burned.

## Usage

1. Deploy the contract on a compatible Ethereum network, specifying the necessary constructor parameters.

2. Interact with the contract using the following functions:

   - `mint`: Call this function to mint new tokens. Pass the recipient's address and the amount of tokens to be minted as parameters.

   - `burn`: Call this function to burn tokens. Provide the address from which tokens should be burned and the amount to be burned as parameters.

3. Access the public variables:

   - `tokenName`: Retrieve the name of the token.

   - `tokenAbbrv`: Retrieve the abbreviation or symbol of the token.

   - `totalSupply`: Retrieve the current total supply of tokens.

4. Retrieve balances:

   - Use the `balances` mapping to retrieve the balance of a specific address.

**Note:** Ensure that you have a compatible Ethereum development environment set up and handle any necessary security considerations when deploying and interacting with the contract.

Remember to comply with the applicable licenses when using this code.
