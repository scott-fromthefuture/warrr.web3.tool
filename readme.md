### _⚠️ This project is not supported or maintained. Use at your own risk._ 

---

![](https://i.imgur.com/0tB0nNn.png)

# wARRR Web3 Tool

The wARRR Web3 tool is a simple interface for interacting with the wARRR contracts on both the Binance Smart Chain and Ethereum networks. It allows users to stake, unstake, and claim rewards, alongside providing useful links related to wARRR. This application is tailored specifically for the MetaMask browser extension and hasn't been tested with other wallets.


## Features

The wARRR Web3 tool is open-source and entirely client-side, making it accessible for anyone to review the code. The application consists of a single, monolithic HTML/JavaScript file - `warrr_tool.html`. This file can be downloaded from [this repoitory](https://github.com/scott-ftf/warrr.web3.tool) and run locally, or simply accessed online via a browser.

To maximize privacy, the app makes only one external request. There are no special fonts, jQuery, or external resources used. All images are inline SVGs. The singular external request is made to fetch `web3.js`, a TypeScript implementation of the Ethereum JSON RPC API and related tooling, maintained by ChainSafe Systems and hosted on [jsDeliver](https://www.jsdelivr.com/package/gh/ethereum/web3.js "jsDeliver") - a free CDN for open source projects.


## Accessing Online

For those who prefer not to run the script locally, the app can simply be accessed online with a browser here:<br />
[https://scott-ftf.github.io/warrr.web3.tool/warrr_tool](https://scott-ftf.github.io/warrr.web3.tool/warrr_tool)


## Using App Locally

The `warrr_tool.html` file can be downloaded from [this repoitory](https://github.com/scott-ftf/warrr.web3.tool) and used locally. To function correctly, **Web3 HTML files need to be served from a web server**. This is because they require *web3 injection into the browser*, which can't occur if the files are opened directly from your local drive in a browser. 

In a Linux operating system, for example, you can create a local server using the following command from the same directory as `warrr_tool.html`: 

```shell 
python3 -m http.server --bind 127.0.0.1 7777
```

This command will serve your files at localhost (127.0.0.1) on port 7777.


## ⚠️ Note to All Users: Carefully Review All MetaMask Prompts

This tool cannot alter your balances on its own. It only sends requests to the web3 wallet. Always check the fees, amounts, and destination addresses in each wallet prompt carefully before approval. This should be a standard procedure when interacting with *any* web3 app.