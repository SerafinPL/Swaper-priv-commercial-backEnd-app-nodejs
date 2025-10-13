# Swaper-priv-commercial-backEnd-app-nodejs
Algo trading bot with Risk-reward management. Swaping crypto on binance by REST api.

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

- MongoDB comunication
- Trading algos:
  - A purchasing algorithm based on three indicators calculated from data from the Binance exchange. Thanks to the implemented indicator analysis, it makes its own decisions about purchases and purchase volumes. The algorithm runs cyclically        every four hours.  
  - The selling algorithm is based on comparing the value of investments retrieved from the MongoDB database. It then analyzes cryptocurrencies and processes those that are at a profit of 2% or more. It then saves the highest profit in the          database and sells when 80% of the highest profit value is reached. The algorithm runs cyclically every 5 minutes. It works similarly to a stop-loss, except that it maximizes profit and secures profit rather than protecting against loss.          
##




