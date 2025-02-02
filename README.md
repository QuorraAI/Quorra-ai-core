# Quorra AI - Core
![Quorra AI](https://github.com/QuorraAI/Quorra-ai-core/blob/main/images/quorra.png?raw=true)

Quorra AI is an adaptive market-making AI designed for Solana's DEX ecosystem.

## AI Market Maker Features
- Token Analysis & Strategy Selection
- AI evaluates key token metrics before market making:
- Market capitalization (Low, Mid, High-cap)
- Trading volumes (distinguishing organic growth from pump & dump)
- Liquidity depth (can narrow spreads be maintained?)
- Number of holders & active traders
- DEX type where the token is listed
- Volatility level (AI chooses aggressive or passive strategies)

## How it works
- AI automatically assigns a "market-making rating" to the token, defining the strategy
- For example, low-cap memecoins require wider spreads, while high-cap tokens need narrower spreads
- AI agent self-learns, comparing token behavior with historical patterns

## Automated Limit Order Optimization
- AI monitors the order book and places orders for maximum efficiency
- Places dynamic limit orders
- Optimizes spreads and order book depth
- Balances buy/sell volumes to keep the market stable

## How it works:
- AI analyzes the last 1000 trades to find ideal entry points
- If liquidity drops → market-making intensifies
- If a whale enters → AI shifts strategy to avoid dumps

## WHO CAN USE THE AI MARKET MAKER?
- Low-cap token projects → Need MM without a massive capital
- Large projects (High-cap) → Want to automate market making
- Traders → Need stable spreads and liquidity
- DeFi platforms → Require automated liquidity management

## TECHNOLOGY STACK
- Solana DEX API: Jupiter, Raydium, Phoenix, Orca, Meteora
- AI & ML: TensorFlow / PyTorch for adaptive strategies
- On-chain analysis: Solana RPC, Helius API
- Backend: Python + Rust (Anchor)

## Features
- Market liquidity analysis
- Smart order placement
- Adaptive strategies for token liquidity

## Installation
```bash
pip install -r requirements.txt
```

## Usage
```bash
python quorra_ai.py
```
