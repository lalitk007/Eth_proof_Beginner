# Eth_proof_Beginner

## MyToken
A simple Solidity smart contract for managing a custom token.
## Requirements
The contract has public variables that store the details about the token:

  -token_Name: Token name (string)
  
  -token_Abbrv: Token abbreviation (string)
  
  -total_Supply: Total supply of the token (uint)
 #
The contract has a mapping of addresses to balances:

bal: Mapping of addresses to token balances (address => uint)

#
The contract has a mint function:

Parameters: address ad - the address to mint tokens to, uint val - the amount of tokens to mint

  -increases the total_Supply by val

  -increases the balance of the ad address by val

#
The contract has a burn function:

Parameters: address ad - the address to burn tokens from, uint val - the amount of tokens to burn

Checks if the balance of the ad address is greater than or equal to val then

  -decreases the total_Supply by val
  
  -decreases the balance of the ad address by val
  

## Usage
Deploy the MyToken contract to a Remix IDE or any solidity supporting enviornment.

Interact with the contract using the following functions:

#
mint: Mint new tokens to an address.

Parameters: address ad - the address to mint tokens to, uint val - the amount of tokens to mint.

Example: mint(address ad, uint val)
#

burn: Burn existing tokens from an address.

Parameters: address ad - the address to burn tokens from, uint val - the amount of tokens to burn.

Example: burn(address ad, uint val)

#
Note: The contract assumes that the deployer has the necessary permissions to mint and burn tokens.


## Authors

- Lalit Kumar


## License

This code is licensed under the MIT License. See the LICENSE file for details.
