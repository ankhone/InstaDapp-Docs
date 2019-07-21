# Getting Started

> InstaDApp has as concept of User Wallets. Before interacting with InstaDApp contracts, Users must create UserWallet though [InstaDApp:Registry](https://etherscan.io/address/0x498b3bfabe9f73db90d252bcd4fa9548cd0fd981)


## Create User Wallet

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')
```

## InstaMaker 

### Open CDP

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```

### Close CDP

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```

### Leverage CDP

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```

### Save CDP

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```

## InstaSwap

### Buy

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```

### Sell

> Sample Description Text

```javascript
require('./env')

const watcher = require('./watcher')


watcher.watchEtherTransfers()
console.log('Started watching Ether transfers')

watcher.watchTokenTransfers()
console.log('Started watching Pluton token transfers\n')

```


## InstaDApp ABIs

### InstaDApp:Registry

```javascript
[{"constant":true,"inputs":[{"name":"_logicAddress","type":"address"}],"name":"logic","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_logicAddress","type":"address"}],"name":"enableStaticLogic","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"","type":"address"}],"name":"logicProxies","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"","type":"address"}],"name":"logicProxiesStatic","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_currentOwner","type":"address"},{"name":"_nextOwner","type":"address"}],"name":"record","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_logicAddress","type":"address"}],"name":"enableLogic","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[],"name":"build","outputs":[{"name":"proxy","type":"address"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_name","type":"string"},{"name":"_userAddress","type":"address"}],"name":"setAddress","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"_logicAddress","type":"address"}],"name":"logicStatic","outputs":[{"name":"","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"_name","type":"string"}],"name":"getAddress","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"","type":"address"}],"name":"proxies","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"_logicAddress","type":"address"}],"name":"disableLogic","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_owner","type":"address"}],"name":"build","outputs":[{"name":"proxy","type":"address"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"inputs":[],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"anonymous":false,"inputs":[{"indexed":true,"name":"sender","type":"address"},{"indexed":true,"name":"owner","type":"address"},{"indexed":false,"name":"proxy","type":"address"}],"name":"Created","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"currentOwner","type":"address"},{"indexed":true,"name":"nextOwner","type":"address"},{"indexed":false,"name":"proxy","type":"address"}],"name":"LogRecord","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"logicAddress","type":"address"}],"name":"LogEnableStaticLogic","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"logicAddress","type":"address"}],"name":"LogEnableLogic","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"logicAddress","type":"address"}],"name":"LogDisableLogic","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"name","type":"string"},{"indexed":false,"name":"addr","type":"address"}],"name":"LogSetAddress","type":"event"}]
```

### InstaCompSave

```javascript
[{"constant":false,"inputs":[{"name":"daiToBorrow","type":"uint256"},{"name":"cTokenAddr","type":"address[]"},{"name":"ctokenFactor","type":"uint256[]"},{"name":"splitAmt","type":"uint256"},{"name":"slippageAmt","type":"uint256"}],"name":"leverage","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"getComptrollerAddress","outputs":[{"name":"troller","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"version","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[{"name":"user","type":"address"},{"name":"ethToFree","type":"uint256"},{"name":"cTokenAddr","type":"address[]"},{"name":"ctokenFactor","type":"uint256[]"}],"name":"getSave","outputs":[{"name":"finalColInEth","type":"uint256"},{"name":"finalDebtInEth","type":"uint256"},{"name":"daiDebt","type":"uint256"},{"name":"isOk","type":"bool"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"getCompOracleAddress","outputs":[{"name":"troller","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":false,"inputs":[{"name":"user","type":"address"},{"name":"daiToBorrow","type":"uint256"},{"name":"cTokenAddr","type":"address[]"},{"name":"ctokenFactor","type":"uint256[]"}],"name":"getLeverage","outputs":[{"name":"finalColInEth","type":"uint256"},{"name":"finalDebtInEth","type":"uint256"},{"name":"ethCol","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"getAddressETH","outputs":[{"name":"eth","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getAddressDAI","outputs":[{"name":"dai","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getCETHAddress","outputs":[{"name":"cEth","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":false,"inputs":[{"name":"ethToFree","type":"uint256"},{"name":"ctokenAddr","type":"address[]"},{"name":"ctokenFactor","type":"uint256[]"},{"name":"splitAmt","type":"uint256"},{"name":"slippageAmt","type":"uint256"}],"name":"save","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"user","type":"address"},{"name":"cTokenAddr","type":"address[]"},{"name":"cTokenFactor","type":"uint256[]"}],"name":"getCompStats","outputs":[{"name":"totalSupply","type":"uint256"},{"name":"totalBorrow","type":"uint256"},{"name":"maxBorrow","type":"uint256"},{"name":"borrowRemain","type":"uint256"},{"name":"maxWithdraw","type":"uint256"},{"name":"ratio","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"getAddressSplitSwap","outputs":[{"name":"splitSwap","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getCDAIAddress","outputs":[{"name":"cDai","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"inputs":[{"name":"_version","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"payable":true,"stateMutability":"payable","type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"srcETH","type":"uint256"},{"indexed":false,"name":"destDAI","type":"uint256"}],"name":"LogSaveCompound","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"srcDAI","type":"uint256"},{"indexed":false,"name":"destETH","type":"uint256"}],"name":"LogLeverageCompound","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"erc20","type":"address"},{"indexed":false,"name":"cErc20","type":"address"},{"indexed":false,"name":"tokenAmt","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogMint","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"erc20","type":"address"},{"indexed":false,"name":"cErc20","type":"address"},{"indexed":false,"name":"tokenAmt","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogRedeem","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"erc20","type":"address"},{"indexed":false,"name":"cErc20","type":"address"},{"indexed":false,"name":"tokenAmt","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogBorrow","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"erc20","type":"address"},{"indexed":false,"name":"cErc20","type":"address"},{"indexed":false,"name":"tokenAmt","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogRepay","type":"event"}]
```

### InstaSave

```javascript
[{"constant":false,"inputs":[{"name":"cdpID","type":"uint256"},{"name":"daiToSwap","type":"uint256"},{"name":"splitAmt","type":"uint256"},{"name":"slippageAmt","type":"uint256"}],"name":"leverage","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[],"name":"version","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"cdpID","type":"uint256"},{"name":"ethToSwap","type":"uint256"}],"name":"getSave","outputs":[{"name":"finalEthCol","type":"uint256"},{"name":"finalDaiDebt","type":"uint256"},{"name":"finalColToUSD","type":"uint256"},{"name":"canSave","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"getAddressKyber","outputs":[{"name":"kyber","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getUniswapMKRExchange","outputs":[{"name":"ume","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getAddressETH","outputs":[{"name":"eth","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getOracleAddress","outputs":[{"name":"oracle","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getAddressDAI","outputs":[{"name":"dai","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getAddressSplitSwap","outputs":[{"name":"splitSwap","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":true,"inputs":[],"name":"getUniswapDAIExchange","outputs":[{"name":"ude","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"constant":false,"inputs":[{"name":"cdpID","type":"uint256"},{"name":"colToSwap","type":"uint256"},{"name":"splitAmt","type":"uint256"},{"name":"slippageAmt","type":"uint256"}],"name":"save","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"cdpID","type":"uint256"},{"name":"daiToSwap","type":"uint256"}],"name":"getLeverage","outputs":[{"name":"finalEthCol","type":"uint256"},{"name":"finalDaiDebt","type":"uint256"},{"name":"finalColToUSD","type":"uint256"},{"name":"canLeverage","type":"bool"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"cdpID","type":"uint256"}],"name":"getMax","outputs":[{"name":"maxColToFree","type":"uint256"},{"name":"maxDaiToDraw","type":"uint256"},{"name":"ethInUSD","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"getSaiTubAddress","outputs":[{"name":"sai","type":"address"}],"payable":false,"stateMutability":"pure","type":"function"},{"inputs":[{"name":"_version","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"payable":true,"stateMutability":"payable","type":"fallback"},{"anonymous":false,"inputs":[{"indexed":false,"name":"what","type":"uint256"},{"indexed":false,"name":"src","type":"address"},{"indexed":false,"name":"srcAmt","type":"uint256"},{"indexed":false,"name":"dest","type":"address"},{"indexed":false,"name":"destAmt","type":"uint256"},{"indexed":false,"name":"beneficiary","type":"address"},{"indexed":false,"name":"minConversionRate","type":"uint256"},{"indexed":false,"name":"affiliate","type":"address"}],"name":"LogTrade","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpID","type":"uint256"},{"indexed":false,"name":"srcETH","type":"uint256"},{"indexed":false,"name":"destDAI","type":"uint256"}],"name":"LogSaveCDP","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpID","type":"uint256"},{"indexed":false,"name":"srcDAI","type":"uint256"},{"indexed":false,"name":"destETH","type":"uint256"}],"name":"LogLeverageCDP","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpNum","type":"uint256"},{"indexed":false,"name":"amtETH","type":"uint256"},{"indexed":false,"name":"amtPETH","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogLock","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpNum","type":"uint256"},{"indexed":false,"name":"amtETH","type":"uint256"},{"indexed":false,"name":"amtPETH","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogFree","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpNum","type":"uint256"},{"indexed":false,"name":"amtDAI","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogDraw","type":"event"},{"anonymous":false,"inputs":[{"indexed":false,"name":"cdpNum","type":"uint256"},{"indexed":false,"name":"daiAmt","type":"uint256"},{"indexed":false,"name":"mkrFee","type":"uint256"},{"indexed":false,"name":"daiFee","type":"uint256"},{"indexed":false,"name":"owner","type":"address"}],"name":"LogWipe","type":"event"}]
```