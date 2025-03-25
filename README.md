📥 Telegram PM: @SkipsTrade   -- message here to purchase the bot
# Solana Bundler Bot

A powerful command-line utility for automating Solana token trading operations through multiple wallets.

## 🔥 Features

- **Multi-wallet Operations**: Create and manage up to 30 wallets at once
- **Auto-Distribution**: Automatically distribute SOL to trading wallets
- **Smart Trading**: Buy and sell tokens with adjustable slippage (up to 50%)
- **Network Support**: Works on Mainnet, Testnet, and Devnet
- **Safety First**: Automated fund recovery after trading
- **Interactive UI**: Easy-to-navigate interface with visual feedback

## 🚀 Quick Start

### Installation

```bash
# install dependincies
cd my_bundler
npm install
```

### Running the Bot

```bash
node bundlerBot.js
```

## 📖 Usage Guide

### Step 1: Prepare the Bundler

1. Select "Prepare bundler" from the main menu
2. Enter the number of wallets to create (1-30)
3. Specify SOL amount per wallet
4. Enter token mint address (example: 4zMMC9srt5Ri5X14GAgXhaHii3GnPAEERYPJgZJDncDU)
5. Confirm to create wallets and distribute SOL

### Step 2: Start Trading

1. Choose "Start bundler (Buy Tokens)" 
2. Confirm to begin trading
3. The bot will use high slippage settings (up to 50%) to ensure trades execute successfully
4. Wait for trades to complete

### Step 3: Sell Tokens

1. Select "Sell tokens & return funds"
2. Choose percentage to sell (25%, 50%, 75%, or 100%)
3. Funds will automatically return to your main wallet

## 💡 Advanced Options

- **Network Selection**: Switch between networks via the "Change network" option
- **Export Wallet**: Backup your bot wallet key for safekeeping
- **Emergency Stop**: Use "Stop the bot" to immediately halt operations and recover funds

## ⚠️ High Slippage Trading

This bot is configured with extended slippage settings (up to 50%) to ensure successful trades even with low-liquidity tokens. The slippage progression works as follows:

1. First attempts lowest slippage (0.5%-5%)
2. If needed, tries medium slippage (6%-20%)
3. For difficult trades, uses high slippage (25%-50%)

## 📝 Configuration

Edit `config.js` to set persistent options:

```javascript
module.exports = {
    MAIN_WALLET_ADDRESS: "Your wallet address here",
    NUM_WALLETS: 5,
    NETWORK: "mainnet-beta"  // "mainnet-beta", "testnet", or "devnet"
};
```

## 🛠️ Troubleshooting

- **UI Issues**: Run `npm install chalk@4.1.2 figlet@1.6.0 ora@5.4.1 cli-table3@0.6.3 boxen@5.1.2`
- **No Route Found**: Try different network or token with more liquidity
- **Transaction Errors**: Ensure you have sufficient SOL in your bot wallet

📥 Telegram PM: @SkipsTrade
