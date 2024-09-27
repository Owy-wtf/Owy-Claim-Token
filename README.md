# Owy-Claim-Token

Owy Claim Token (OWYC) is the token distributed to all presale participants to claim their Owy after the event ends. The contract is derived from [Openzeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol) contract for security purpose.

## Guide

### 1.Get foundry

Head over to [foundry book](https://book.getfoundry.sh/) and complete installation and setup

### 2.Set up repo

Open terminal and clone the repo

```bash
git clone https://github.com/Owy-wtf/Owy-Claim-Token.git
```

Enter the downloaded repo

```bash
cd Owy-Claim-Token
```

### 3.Build

Paste the below command line to the terminal

```bash
forge build
```

_Building configuration can be found in `foundry.toml` file._

### 4.Deployment

Add your info to the command below and paste them to the terminal. Leave some Eth or native-chain token in the wallet to succeed deployment.

The command below will automatically compile all contracts and deploy to the blockchain.

**Make sure to keep your wallet private key securely, do not expose to anyone during and after deployment**

```bash
forge create --rpc-url <your_rpc_url> \
    --private-key <your_private_key> \
    --etherscan-api-key <your_etherscan_api_key> \
    --verify \
    src/OWYC.sol:OWYC
```

### 5.Clean

Clean the repo and you're done ~

```bash
forge clean
```

## Contribution and Use

Note that we use `evem_version = "cancun"`, this may or may not work for other versions and we do not encourage such modification.

We do not give any warranties and will not be liable for any loss incurred through any use of this codebase.

Please always include your own thorough tests when using this codebase to make sure it works correctly with your code.

## Acknowledgement

We would love to thank

> [Openzeppelin](https://github.com/OpenZeppelin/openzeppelin-contracts)

for providing these open-source smart contracts for public use and sincerely appreciate their contribution to improve security and user-experience in the blockchain industry :heart:.

==_This repository is open-sourced under the MIT license._:smile: Enjoy building!==
