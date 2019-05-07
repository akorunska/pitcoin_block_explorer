# pitcoin_block_explorer

This a simple prototype of bitcoin and a block explorer for it.

## Build Setup

First, set up pitcoin node. Code and instuctions can be found in `pictoin_mainnet_node_edition` folder.


Than, go to `pitcoin_block_explorer` folder and run following:

``` 
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

If you are building the whole thing on the raspberry (or not from localhost in general), remember to edit config/index.js.

All you have to do is modify the port value inside the dev block:

```
 dev: {
    assetsSubDirectory: 'static',
    assetsPublicPath: '/',
    proxyTable: {},

    host: '10.86.1.3',
    port: 8080, 
    autoOpenBrowser: false,
    errorOverlay: true,
    notifyOnErrors: true,
    poll: false,

```

Modify node port in src/settings.js and in pitcoin_modules/settings.py (for pitcoin node).

