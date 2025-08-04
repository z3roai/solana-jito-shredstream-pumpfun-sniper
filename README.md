# 🌟🚀⚡ Jito Shredstream Pumpfun Sniper 🌟🚀⚡

## 🎯 About Pumpfun Sniper
Welcome to our advanced Pumpfun sniper! This sophisticated tool enables you to snipe newly launched tokens on Pumpfun with exceptional speed and precision. Our solution provides a competitive edge in the fast-paced world of token sniping.

## ⚡ Jito ShredStream vs GRPC Performance
Our Jito shredstream pumpfun sniper delivers outstanding performance with 0-block sniping capabilities. We achieve an impressive 70-80% win rate as the first buyer, thanks to Jito shredstream's superior speed advantage of 100-150ms over traditional GRPC methods. This significant latency reduction dramatically increases your chances of winning against competitors using standard GRPC connections.

## 📊 Test Examples & Proof of Concept
We've successfully tested our system with real transactions:

**Token Creation Transaction:** https://solscan.io/tx/5nkZDeGwt4T22oKXX1vDHEQtC1sY5qpYapGgryUrNk5Q64L1Fjv57aNiFQfmVfKTQgUTi6mEeFBPfotygCbFAWKM

**Successful Buy Transaction:** https://solscan.io/tx/5wegzb5MsJ32k5M655iyB8eehwRuV4yVFg1D5szEUuz8kGbJoW3RFLtr3mFDmvP4x5epujLA38VF2h2Hhac5rh71

## ✨ Key Features
🎯 **Real-time transaction monitoring via Jito Shredstream** - Experience lightning-fast transaction detection
<br>
💰 **Low-tip transaction detection (configurable threshold)** - Optimize your trading costs with smart tip filtering
<br>
🤖 **Automated sniping with buy & sell strategies** - Let our intelligent system handle your trading decisions
<br>
⚡ **Redis caching for performance optimization** - Enjoy blazing-fast response times with our caching system
<br>
🔧 **Customizable parameters (price range, tip limits, delays)** - Tailor the system to your specific trading preferences
<br>

## 🛠️ Setup & Installation

### 📋 Prerequisites
- **Rust** (v1.70+ recommended) - Our preferred programming language for optimal performance
- **Redis** (for caching) - Essential for maintaining high-speed operations
- **Solana CLI** (optional, for wallet management) - Useful for additional wallet operations

### 📥 Installation Steps

#### Step 1: Clone the Repository
```bash
git clone https://github.com/TakhiSol/jito-shredstream-pumpfun-sniper.git
cd jito-shredstream-pumpfun-sniper
```

#### Step 2: Build the Project
```bash
cargo build --release
```

## ⚙️ Configuration

### Environment Setup
Create a `.env` file in the root directory with the following carefully configured variables:

```env
# Jito Shredstream Endpoint (default: local Jito validator)
SERVER_URL="http://127.0.0.1:9999"

# Solana RPC (use a private RPC for lower latency)
RPC_URL="https://api.mainnet-beta.solana.com"

# Wallet Private Key (Base58 format)
PRIVATE_KEY="your_private_key_here"

# Redis Cache (improves performance significantly)
REDIS_URL="redis://127.0.0.1:6379"

# Trading Parameters (customize according to your strategy)
MIN_SOL_PRICE="0.5"    # Minimum token price in SOL to snipe
MAX_SOL_PRICE="3.0"    # Maximum token price in SOL to snipe
BUY_SOL_AMOUNT="0.1"   # SOL amount per snipe transaction
SELL_DELAY_MS="5000"    # Delay before selling in milliseconds
MAX_TIP_LAMPORTS="10000" # Maximum tip allowed in lamports
```

## 🚀 Usage Guide

### Running the Sniper
To start your sniping operations, simply run:
```bash
cargo run --release
```

## 🎯 Custom Strategy Development

### Modifying Trading Logic
You can customize your trading strategies by modifying `src/utils/auto_trader.rs` to adjust:

- **Buy conditions** (e.g., liquidity thresholds, market analysis)
- **Sell timing** (dynamic delays, trailing stops, profit targets)
- **Tip filtering** (aggressive vs. conservative approaches)

## ⚡ How Our System Works

### Step-by-Step Process
1. **Real-time Monitoring** - Our system continuously listens to Jito Shredstream for new transactions
2. **Smart Detection** - We detect low-tip transactions (below your configured MAX_TIP_LAMPORTS threshold)
3. **Token Analysis** - The system analyzes swaps for tokens within your specified price range (MIN_SOL_PRICE to MAX_SOL_PRICE)
4. **Automated Execution** - Executes buys with your configured BUY_SOL_AMOUNT
5. **Intelligent Selling** - Automatically sells after your specified SELL_DELAY_MS

## ⚠️ Important Notes & Safety Warnings

### Risk Management
⚠️ **High-risk trading alert:** Sniping can lead to potential losses due to slippage, rug pulls, and failed transactions
<br>
⚠️ **Wallet security:** We strongly recommend using a dedicated wallet for sniping operations
<br>
⚠️ **RPC optimization:** A private RPC connection is essential for achieving optimal sniping performance

## 🔧 Advanced Performance Optimizations

### Server Recommendations
- **Low-latency hosting:** Consider running on AWS/GCP servers in us-west-1 for optimal performance
- **Redis optimization:** Preload token metadata in Redis to accelerate lookups
- **Dynamic fee adjustment:** Implement smart gas fee adjustments based on network congestion

## 🤝 Community & Support

### Contributing
We warmly welcome contributions from the community! Please feel free to open an issue or submit a pull request for any improvements or suggestions.

### Get in Touch
We're always here to help! Feel free to reach out with any questions, suggestions, or feedback. Your input is invaluable to us.

**📱 Telegram:** [Takhi77](https://t.me/hi_3333)

---

*Thank you for choosing our Jito Shredstream Pumpfun Sniper! We hope this tool helps you achieve your trading goals safely and effectively.* 🌟
