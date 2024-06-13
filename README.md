# MyToken Smart Contract

## Overview

MyToken is a simple ERC-20 compatible smart contract written in Solidity. It supports minting and burning of a custom token named Swastik (abbreviation: Swa).

## Contract Details

- **Token Name:** Swastik
- **Token Abbreviation:** Swa
- **Compiler Version:** 0.8.26

## Functions

### `mint(address _address, uint256 _value)`

Mints `_value` tokens to `_address`.

```solidity
function mint(address _address, uint256 _value) public {
totalSupply += _value;
balances[_address] += _value;
}
function burn(address _address, uint256 _value) public {
if (balances[_address] >= _value) {
totalSupply -= _value;
balances[_address] -= _value;
}
}
myToken.mint(0xYourAddress, 1000);
myToken.burn(0xYourAddress, 500);

License

This project is licensed under the MIT License. See the LICENSE file for details.

Author Swastik
