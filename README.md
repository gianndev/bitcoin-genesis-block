# Bitcoin Genesis Block

What does the Bitcoin genesis block contain? Have you ever wondered? Surely you have heard that Satoshi Nakamoto hid in the block a quote from an article in the British newspaper *The Times* of January 3, 2009. And you probably believed it because a friend told you, or you read it on a forum or your favorite YouTuber said it. But if there is one rule in the world of cryptocurrencies it is: **"dont trust, verify"**.

In this repository you will learn step by step how you too can verify for yourself what Nakamoto actually hid in the genesis block to understand if what you heard is true or not. Don't worry, you will discover that it is a very simple thing and requires only a few steps. Follow my commands carefully and you too will be able to put into practice the motto **"dont trust verify"**.

Have fun 😎!

## STEP 1: Getting the first block from the blockchain

What we need to do is go and retrieve the first block of the Bitcoin blockchain. Now in theory what we should do is download the entire blockchain by requesting it from some node, but in addition to being complicated for beginners and time-consuming, currently (June 2025) **the Bitcoin blockchain takes up about 652GB of space**, which... Well, not everyone has such a hard drive. For what we need to do, that is, take a look at the first block, it is sufficient to download just the "initial part" of the blockchain without everything else.

### 1.1 Install Bitcoin Core

Bitcoin by definition is a software, so to work with Bitcoin we need to install a software. The software in question is called *Bitcoin Core* and it is officially the software that runs the Bitcoin protocol. 

Follow the instructions to install *Bitcoin Core* on your operating system. When following these instructions, feel free to choose whether to download the CLI (command line only) or GUI (graphical interface) version. For example, I chose to download the terminal version.

#### **Windows**

Download the installer from [bitcoincore.org](https://bitcoincore.org/) and follow the instructions

To verify the installation, open the command-prompt and type:  

```bash
bitcoin-cli --version
```

#### **MacOS**

Use [Homebrew](https://brew.sh/):  

```bash
brew install bitcoin
```

Homebrew installs packages in a dedicated directory (e.g. `/opt/homebrew`) and creates automatic symlinks. Check with:
 
```bash
bitcoin-cli --version
```

#### **Linux (Ubuntu/Debian)**

Install Bitcoin Core and necessary dependencies:

```bash
sudo apt install bitcoind jq xxd # Bitcoin CLI + decoding tools
```

If you prefer GUI:

```bash
sudo apt install bitcoin-qt
```

Verify installation:

```bash
bitcoind --version
``` 

---

> NOTE: I have tested my tutorial firsthand on my Windows and Ubuntu devices, so for MacOS or other Linux distros there may be some inaccuracies. If you find any problems feel free to open an issue to report it.