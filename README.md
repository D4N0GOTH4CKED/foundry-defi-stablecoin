##  Foundry Defi StableCoin
[DSCEngine Example](https://sepolia.etherscan.io/address/0x091ea0838ebd5b7dda2f2a641b068d6d59639b98#code)
[Decentralized Stablecoin Example](https://sepolia.etherscan.io/address/0xf30021646269007b0bdc0763fd736c6380602f2f#code)

# About

This project is meant to be a stablecoin where users can deposit WETH and WBTC in exchange for a token that will be pegged to the USD.

## Design of our protocol
1. (Relative Stablility) Achored or Pegged -> $1.00 ( Our coin will be equivalent to one dollar  )
- We use Chainlink Price Feed to make sure it is pegged to $1.00
- After getting priceFeed, we set a function to exhange ETH $  BTC -> $1.00
2. Stability Mechanism (Minting): Algorithmic  (Decentralized) - This going to be decentralized( 100% on chain )
- People can only mint stablecoin with enough collateral (coded)
3. Collateral: Exogeneous(Crypto)
   1. wETH
   2. wBTC

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

- **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
- **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
- **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
- **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```
