# Bitcoin Genesis Block

What does the Bitcoin genesis block contain? Have you ever wondered? Surely you have heard that Satoshi Nakamoto hid in the block a quote from an article in the British newspaper *The Times* of January 3, 2009. And you probably believed it because a friend told you, or you read it on a forum or your favorite YouTuber said it. But if there is one rule in the world of cryptocurrencies it is: **"dont trust, verify"**.

In this repository you will learn step by step how you too can verify for yourself what Nakamoto actually hid in the genesis block to understand if what you heard is true or not. Don't worry, you will discover that it is a very simple thing and requires only a few steps. Follow my commands carefully and you too will be able to put into practice the motto **"dont trust verify"**.

Have fun 😎!

## STEP 1: Getting the first block from the blockchain

What we need to do is go and retrieve the first block of the Bitcoin blockchain. Now in theory what we should do is download the entire blockchain by requesting it from some node, but in addition to being complicated for beginners and time-consuming, currently (June 2025) **the Bitcoin blockchain takes up about 652GB of space**, which... Well, not everyone has such a hard drive. For what we need to do, that is, take a look at the first block, it is sufficient to download just the "initial part" of the blockchain without everything else.

### 1.1 Install Bitcoin Core

Bitcoin Core is the reference implementation of the Bitcoin protocol. To install, simply go to the official download page and pick the version that matches your system and preference (CLI or GUI):

👉 [https://bitcoincore.org/en/download/](https://bitcoincore.org/en/download/)

Follow the on‑screen instructions there for Windows, macOS, or Linux; the page includes checksums and signature‑verification steps to ensure you get an authentic, up‑to‑date build.

> **Tip:**
>
> * If you plan to script or interact programmatically, choose the **CLI** (command‑line) version.
> * If you prefer a graphical wallet with point‑and‑click, choose the **GUI** (Bitcoin Qt) version.

### 1.2 Download only the first 20 blocks

TODO