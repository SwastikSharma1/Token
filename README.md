# MyToken Smart Contract

## Overview

MyToken is a basic token contract on the Ethereum blockchain.

- **Token Name:** Swastik
- **Token Symbol:** Swa
- **Total Supply:** 0 initially

## Functionalities

### mint

```solidity
function mint(address _address, uint256 _value) public
```

- Increases total supply and balances of `_address` by `_value`.

### burn

```solidity
function burn(address _address, uint256 _value) public
```

- Decreases total supply and balances of `_address` by `_value`, if the address has enough tokens.

## Usage

1. **Minting Tokens:**
   ```solidity
   mint(0xYourAddress, 100);
   ```

2. **Burning Tokens:**
   ```solidity
   burn(0xYourAddress, 50);
   ```

## Author

Swastik

## License

MIT License
