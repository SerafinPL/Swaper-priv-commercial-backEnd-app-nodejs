# Swaper backEnd app
Algo trading bot with Risk-reward management. Swaping crypto on varius exchanges by REST api.
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

- **Risk and reward management algorithm** - The implemented strategy calculates the profit/loss of a position relative to the total capital and the overall profit/loss of the capital. The algorithm compares the defined levels of accepted risk and reward relative to the position and capital. On this basis, it makes independent decisions about the possible exit from a particular position or the entire investment.
- Trading algos:
  - **A purchasing algorithm** based on three indicators calculated using data from the varius exchanges. Thanks to the implemented indicator analysis, it makes independent decisions regarding purchases and purchase volumes. The algorithm is executed cyclically according to a set number of hours.
  - **The selling algorithm** is based on a comparison of investment values taken from the database and current market data. The algorithm analyzes the current value of individual investments, and those that generate a profit of x*% or higher are processed further. For selected positions, the algorithm saves the “highest profit” in the database. In subsequent cycles, it sells positions after reaching x*% of the ‘highest profit’ value or raises the ‘highest profit’ value. The algorithm is executed cyclically according to a set number of minutes. It works similarly to a raising stop-loss order.
- REST API comunication with: Binance, Kraken, KuCoin.
- API to comunicate with client app.
- MongoDB comunication

[ x* ] - x is a ingteger
##

 ![Logo](https://kubakoder.pl/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Ffavicon.5d6e1adf.png&w=48&q=75)

### 👨🏻‍💻 Author: [@SerafinPL](https://www.github.com/serafinpl)

### 🌐 Author URI: [http://kubakoder.pl](http://kubakoder.pl)
##

### Roadmap

- ![Static Badge](https://img.shields.io/badge/okx-api-ex?style=plastic&logo=okx&labelColor=%23000000&color=%23ffffff) instgration.
