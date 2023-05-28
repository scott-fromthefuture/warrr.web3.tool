
![](https://i.imgur.com/0tB0nNn.png)

# wARRR Web3 Tool

This app is a interface for interacting with the wARRR contracts on both the Binance Smart Chain and Ethereum networks. Stake, unstake, and claim rewards, also provides useful links related to wARRR. This was made specifically for the MetaMask browser extension and hasn't been tested with other wallets.

Consists of a single monolithic HTML/JavaScript file - `warrr_tool.html`, making it easy to review teh client side code. 

External requests are limited to one. No special fonts, jQuery, or external resources used. All images are inline SVGs. The external request is made to fetch `web3.js`, a TypeScript implementation of the Ethereum JSON RPC API and related tooling, maintained by ChainSafe Systems and hosted on [jsDeliver](https://www.jsdelivr.com/package/gh/ethereum/web3.js "jsDeliver") - a free CDN for open source projects. All communication is otherwise directly via the web3 wallet.


## Accessing Online

The app can be accessed online with a browser here:<br />
[https://scott-ftf.github.io/warrr.web3.tool/warrr_tool](https://scott-ftf.github.io/warrr.web3.tool/warrr_tool)


## Using App Locally

The `warrr_tool.html` file can be downloaded from [this repoitory](https://github.com/scott-ftf/warrr.web3.tool) and used locally. To function correctly, Web3 HTML files need to be served from a web server. They require *web3 injection into the browser*, which can't occur if the files are opened directly from your local file system in a browser. 

In a Linux operating system, for example, you can create a local server using the following command from the same directory as `warrr_tool.html`: 

```shell 
python3 -m http.server --bind 127.0.0.1 7777
```

This command will serve the app at localhost (127.0.0.1) on port 7777.<br />
[http://127.0.0.1:7777/warrr_tool.html](http://127.0.0.1:7777/warrr_tool.html)



## ⚠️ Note to All Users: Carefully Review All MetaMask Prompts

This tool cannot alter your balances on its own. It only sends requests to the web3 wallet. Always check the fees, amounts, and destination addresses in each wallet prompt carefully before approval. 

This project is not supported or maintained, so please use at our own risk.