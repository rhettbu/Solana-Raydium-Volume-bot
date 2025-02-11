# 🚀 Solana Raydium Volume Bot – Automated Liquidity & Trading Volume Booster

![GitHub stars](https://img.shields.io/github/stars/rhettbu/solana-raydium-volume-bot?style=social)
![Solana](https://img.shields.io/badge/Solana-Raydium%20Bot-purple)

## 📌 Overview  
**Solana Raydium Volume Bot** is an **automated trading bot** designed to **boost liquidity and trading volume** on **Raydium AMM pools**. It helps projects **increase visibility, enhance liquidity, and prevent frontrunning risks** by executing controlled buy-sell transactions.  

### ✅ **Key Features**
- **📈 Automated Buy & Sell Trading** – Generates volume on selected Raydium liquidity pools.  
- **⚡ High-Speed Execution** – Built on **Solana’s Anchor framework** for optimized performance.  
- **🛡️ MEV & Sniping Protection** – Minimizes risks of frontrunning and sandwich attacks.  
- **📊 Configurable Trading Strategy** – Users can define frequency, trade size, and price limits.  
- **🌍 Multi-Pair Support** – Works across multiple Raydium liquidity pools.  
- **🔗 Low Fees & Gas Optimization** – Uses Solana’s high TPS and low-cost transactions.  

---

## 🚀 **Installation & Setup**

### **🔹 Prerequisites**
Ensure you have the following installed:
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli)
- [Node.js](https://nodejs.org/en/download/)
- [Rust & Anchor](https://project-serum.github.io/anchor/getting-started/installation.html)

### **🔹 Clone the Repository**
```sh
git clone https://github.com/rhettbu/solana-raydium-volume-bot.git
cd solana-raydium-volume-bot


## Usage Instructions

1. **Clone the Repository**

   ```
   git clone https://github.com/rhettbu/Solana-Raydium-Volume-Bot.git
   cd Solana-Raydium-Volume-Bot
   ```

2. **Install Dependencies**

   ```
   npm install
   ```

3. **Set Up Environment Variables**
   Rename `.env.example` to `.env` and configure it with your RPC and WSS URLs, the main wallet's secret key, and the jito auth keypair.

4. **Launch the Bot**
   ```
   npm run start
   ```

## Comparison with Previous Versions

### Drawbacks of the Previous Version

- **Static Wallet Usage**: Utilized fixed wallets for transactions, making the trading pattern obvious on DexScreener.
- **Lack of Maker Diversity**: Did not contribute to an increase in the number of market makers, only the volume.
- **Inefficient Token Management**: Tokens were accumulated in the main wallet without being sold first.
- **Balanced Buy/Sell Transactions**: Each cycle ended with a sell, creating downward price pressure.

## Enhancements in the Current Version

- **Dynamic SOL Transfers**: Transfers SOL to a new wallet after each buy-sell cycle.
- **Increased Maker Participation**: Generates new wallets continuously, enhancing market maker diversity.
- **Prioritized Selling**: Sells remaining tokens before gathering SOL, optimizing the use of funds.
- **Buy Dominance**: Executes two buys for every sell, fostering greater buying pressure.
- **Extensive Customization**: Allows detailed configuration to suit various operational needs.

## Contact Information

For inquiries, contact me via [Telegram](https://t.me/rhettjel) or Discord at @monkalche and [Twitter](https://x.com/defai_maxi).

If you need assistance with other trading bots, I also specialize in developing advanced solutions such as the Raydium and Pumpfun sniper, Raydium bundler, Pumpfun bundler, Shit-token launcher, Token-freezer, and market-making bots. Additionally, I offer both console-based and Telegram-integrated versions tailored to your specific needs. Feel free to reach out to discuss your requirements!
