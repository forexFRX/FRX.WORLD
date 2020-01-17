![FRX.WORLD](images/logo.png)

# Forex Token

## Overview


### Etherscan.io
```
https://etherscan.io/token/0x2FEeb86860b42BfD84D22111d360246E7E9e8257
```

### Token Address 
```
0x2FEeb86860b42BfD84D22111d360246E7E9e8257
```

### Forex Token

The Forex token `FRXToken.sol` is ERC-20 standard compatible and has the following additional characteristics:

1. An initial amount of 500,000,000 FRX tokens supply.
2. An ability to burn tokens by users to reduce total number of token supply.

FRX.WORLD plans to do the following:

- Burn all unallocated tokens to proportionally increase each token holder’s percentage in the overall token amount.

#### Implementation

We use [OpenZeppelin](https://openzeppelin.org) code for `SafeMath`, `Ownable`, `Burnable` and `StandardToken` logic.

* `SafeMath` provides arithmetic functions that throw exceptions when integer overflow occurs.
* `Ownable` keeps track of a contract owner and permits the transfer of ownership by the current owner.
* `Burnable` provides a burn function that decrements the balance of the burner and the total supply.
* `StandardToken` provides an implementation of the ERC-20 standard.

The token contract includes the following constants:

```javascript
    name             = "Forex";
    symbol           = "FRX";
    decimals         = 8;
    INITIAL_SUPPLY   = 500 million FRX;
    Mintable         = False
```

The above constants indicate a maximum supply of 500 million tokens.

© 2020 FRX.WORLD. All Rights Reserved.
