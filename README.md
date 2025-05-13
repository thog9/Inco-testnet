# Inco Testnet Scripts

This repository contains a collection of Python scripts designed to interact with the Inco Testnet, a blockchain test network for decentralized applications. The main script, main.py, provides a user-friendly command-line interface (CLI) to execute various operations on the Inco Testnet, such as minting tokens, shielding/unshielding USDC, deploying smart contracts, and sending transactions. Built with web3.py, the scripts support asynchronous execution and offer bilingual output (English and Vietnamese) for enhanced user interaction.

Faucet: [Herafi Testnet Faucet](https://testnet.herafi.xyz/faucet)

## ✨ Features Overview

### General Features

- **Multi-Account Support**: Reads private keys from `pvkey.txt` to perform actions across multiple accounts.
- **Colorful CLI**: Uses `colorama` for visually appealing output with colored text and borders.
- **Asynchronous Execution**: Built with `asyncio` for efficient blockchain interactions.
- **Error Handling**: Comprehensive error catching for blockchain transactions and RPC issues.
- **Bilingual Support**: Supports both English and Vietnamese output based on user selection.

### Included Scripts

1. **Mint USDC**: Mints USDC tokens on the Inco Testnet.
2. **Mint cUSDC**: Mints cUSDC tokens on the Inco Testnet.
3.**Shield USDC ➯ cUSDC**: Converts USDC to cUSDC via a shielding contract.
4.**Unshield cUSDC ➯ USDC**: Converts cUSDC back to USDC via an unshielding contract.
5.**Deploy Smart Contract Mintair**: Deploys the Mintair smart contract on the Inco Testnet.
6.**Send TX (Random or File)**: Sends random transactions or transactions to addresses listed in `address.txt`.
7.**Deploy Token Smart Contract**: Deploys an ERC20 token smart contract on the Inco Testnet.
8.**Send Token ERC20 (Random or File)**: Sends ERC20 tokens to random addresses or addresses listed in `addressERC20.txt`.
9.**Deploy NFT Smart Contract**: Deploys an NFT smart contract on the Inco Testnet.

## Prerequisites

Before running the scripts, ensure you have the following installed:

- Python 3.8+
- `pip` (Python package manager)
- **Dependencies**: Install via `pip install -r requirements.txt` (ensure `web3.py`, `colorama`, `asyncio`, `eth-account`, `aiohttp_socks` and `inquirer` are included).
- **pvkey.txt**: Add private keys (one per line) for wallet automation.
- Access to the Inco Testnet RPC (e.g., https://sepolia.base.org or Inco-specific RPC).
- **proxies.txt** (optional): Add proxy addresses for network requests, if needed.

## Installation

1. **Clone this repository:**
- Open cmd or Shell, then run the command:
```sh
git clone https://github.com/thog9/Inco-testnet.git
```
```sh
cd Inco-testnet
```
2. **Install Dependencies:**
- Open cmd or Shell, then run the command:
```sh
pip install -r requirements.txt
```
3. **Prepare Input Files:**
- Open the `pvkey.txt`: Add your private keys (one per line) in the root directory.
```sh
nano pvkey.txt 
```
- Open the `address.txt`(optional): Add recipient addresses (one per line) for `sendtx.py`, `nftcollection.py`, `deploytoken.py`, `sendtoken.py`, `proxies.txt`.
```sh
nano address.txt 
```
```sh
nano addressERC20.txt
```
```sh
nano contractNFT.txt
```
```sh
nano proxies.txt
```
```sh
nano contractERC20.txt
```
4. **Run:**
- Open cmd or Shell, then run command:
```sh
python main.py
```
- Choose a language (Vietnamese/English).

## Contact

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099) 

----

BUYMECAFE: [BUY ME CAFE](https://buymecafe.vercel.app/)
