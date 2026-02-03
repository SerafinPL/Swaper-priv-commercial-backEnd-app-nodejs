# Swaper back-end app
Algo trading bot with Risk-reward management. Swaping crypto on various exchanges by REST api.
##

### 🛠️ Stack: 

![Static Badge](https://img.shields.io/badge/linux-mint-xfce?style=plastic&logo=linuxmint)
![Static Badge](https://img.shields.io/badge/git_at_-github-ex?style=plastic&logo=git&logoColor=F05032&color=F05032)

![Static Badge](https://img.shields.io/badge/nodejs-22.20.0-ex?style=plastic&logo=nodedotjs)
![Static Badge](https://img.shields.io/badge/typescript-5.8.3-ex?style=plastic&logo=typescript&logoColor=3178C6&color=3178C6)
![Static Badge](https://img.shields.io/badge/axios-1.10.0-ex?style=plastic&logo=axios&logoColor=%235A29E4&color=%235A29E4)

![Static Badge](https://img.shields.io/badge/dotenv-16.5.0-ex?style=plastic&logo=dotenv&color=%23ECD53F)
![Static Badge](https://img.shields.io/badge/express.js-5.1.0-ex?style=plastic&logo=express&labelColor=%23000&color=%23fff)
![Static Badge](https://img.shields.io/badge/mongodb-6.17.0-ex?style=plastic&logo=mongodb&labelColor=%23000&color=%23fff)
##

### Features

- **Risk & Reward management algorithm** - The implemented strategy calculates the profit/loss of a position relative to the total capital and the overall profit/loss of the capital. The algorithm compares the defined levels of accepted risk and reward relative to the position and capital. On this basis, it makes independent decisions about the possible exit from a particular position or the entire investment.
- Trading algos:
  - **A purchasing algorithm** based on three indicators calculated using data from the various exchanges. Thanks to the implemented indicator analysis, it makes independent decisions regarding purchases and purchase volumes. The algorithm is executed cyclically according to a set number of hours.
  - **The selling algorithm** is based on a comparison of investment values taken from the database and current market data. The algorithm analyzes the current value of individual investments, and those that generate a profit of x*% or higher are processed further. For selected positions, the algorithm saves the “highest profit” in the database. In subsequent cycles, it sells positions after reaching x*% of the ‘highest profit’ value or raises the ‘highest profit’ value. The algorithm is executed cyclically according to a set number of minutes. It works similarly to a raising stop-loss order.
- REST API communication with: Binance, Kraken, KuCoin.
- API to communicate with client app.
- MongoDB communication

[ x* ] - x is a ingteger
##

 ![Logo](https://kubakoder.pl/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Ffavicon.5d6e1adf.png&w=48&q=75)

### 👨🏻‍💻 Author: [@SerafinPL](https://www.github.com/serafinpl)

### 🌐 Author URI: [http://kubakoder.pl](http://kubakoder.pl)
##

### Roadmap

to do:
- [ ] OAuth integration required to make the application available to beta testers
- [ ] remake invest data structure to work with more than one user
- [ ] remake Risk & Reward management data structure to work with more than one user
- [ ] ![Static Badge](https://img.shields.io/badge/okx-api-ex?style=plastic&logo=okx&labelColor=%23000000&color=%23ffffff) integration
- [ ] Make nextAuth & MongoDb integration

      
in progress:
      
done:

Ver 0.7 - independent trading app with Risk & Reward management mode

Ver 0.6 - independent trading app with Risk & Reward management mode
- [x] review of the entire application code
- [x] error handling and saving logs in database about issues
- [x] some modifications was required for migration to vps

Ver 0.5 - independent trading app with Risk & Reward management mode
- [x] removal of the implementation of the connection with the near protocol
- [x] run a Risk & Reward management with time cycles on binance
- [x] development & implementation of a Risk & Reward management algorithm and data structure

Ver 0.4 - independent purchasing & selling app
- [x] run a purchasing algorithm with time cycles on binance
- [x] migration invest data from Near Protocol to MongoDB
- [x] integration with new data base provider ![Static Badge](https://img.shields.io/badge/mongodb-6.17.0-ex?style=plastic&logo=mongodb&labelColor=%23000&color=%23fff)
- [x] some changes of complex assessment and indicator ranks algorithms and add Price Trend to calculations after testing feedback
- [x] calculate Price Trend from clines kraken & binance data
- [x] testing with actual market data and back testing complex assessment and indicators ranks functions
- [x] make API to get candlestick data and calculated indicator & ranks from all 3 exchanges by client app
- [x] development & implementation of a complex assessment based on three indicators
- [x] development & implementation of a rank algorithm for 'indicator 3' calculations
- [x] calculate 'indicator 3' from candlestick kraken & binance data
- [x] calculate all 2 indicators from candlestick binance data
      
Ver 0.3 - independent better selling app
- [x] extend the sales algorithm with the “highest profit” stop loss functionality
- [x] run a selling algorithm with time cycles on binance
- [x] add binance to APIs
- [x] ![Static Badge](https://img.shields.io/badge/binance-api-ex?style=plastic&logo=binance&logoColor=%23F0B90B&labelColor=%23000&color=%23F0B90B) integration
- [x] development & implementation of a rank algorithm for 'indicator 2' calculations
- [x] development & implementation of a rank algorithm for 'indicator 1' calculations
- [x] calculate 'indicator 2' from candlestick kraken data
- [x] calculate 'indicator 1' from candlestick kraken data
- [x] expand API to make purchase on more than one exchanges by client app
      
Ver 0.2 - independent selling app
- [x] run a selling algorithm with time cycles on kraken
- [x] development & implementation of a selling algorithm 
- [x] expand API to get & set invest data by client app with more than one exchanges
- [x] remake invest data structure to work with more than one exchanges
- [x] make API to get invest and kucoin data at once by client app
- [x] ![Static Badge](https://img.shields.io/badge/kucoin-api-ex?style=plastic&logo=kucoin&labelColor=%23000&color=%2301BC8D) read only integration
- [x] make API to make purchase on kraken by client app 
- [x] make API to get invest and kraken data at once by client app
- [x] make API to get & set invest data by client app
      
Ver 0.1 - starting app
- [x] ![Static Badge](https://img.shields.io/badge/near-contract-ex?style=plastic&logo=near&labelColor=%23000&color=%23fff) integration as data base
- [x] ![Static Badge](https://img.shields.io/badge/kraken-api-ex?style=plastic&labelColor=%235841D8&color=%23000) integration
- [x] ![Static Badge](https://img.shields.io/badge/nodejs-22.20.0-ex?style=plastic&logo=nodedotjs) ![Static Badge](https://img.shields.io/badge/typescript-5.8.3-ex?style=plastic&logo=typescript&logoColor=3178C6&color=3178C6) ![Static Badge](https://img.shields.io/badge/dotenv-16.5.0-ex?style=plastic&logo=dotenv&color=%23ECD53F) startup config

