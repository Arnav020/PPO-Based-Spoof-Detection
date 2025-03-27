# 🚀 PPO-Based Spoof Detection in Algorithmic Trading

## 🔍 Overview
This advanced deep reinforcement learning model is designed to catch market manipulation in action! It scans Level 3 Limit Order Book (LOB) data to detect spoofing patterns—where traders place and cancel large orders to create artificial price swings. Our model is built to recognize these deceptive tactics, especially during high-volatility events like the LUNA flash crash of May 2022.

## 🛠️ How It Works
### 📊 Data Preprocessing
- Cleans and structures raw Level 3 LOB data for analysis.
- Extracts key attributes and temporal patterns.
- Includes robust error handling to ensure real-world applicability.

### 🚀 Feature Engineering
Our model goes beyond basic detection with specialized features:
- Rolling statistics on price and size movements.
- Order flow imbalance metrics.
- Cancellation ratios to identify suspicious behavior.
- Time-sensitive features to capture rapid market shifts.

### 🎮 Market Simulation Environment
- Dynamic spoofing threshold adjustments.
- Realistic reward mechanisms for reinforcement learning.
- State representation that tracks evolving market conditions.

### 🧠 PPO Policy Network
- Uses deep learning to process time-series financial data.
- Outputs real-time spoofing/non-spoofing classifications.
- Continuously adapts to shifting market trends.

### 📈 Training & Evaluation
- Collects experience efficiently to speed up learning.
- Implements robust advantage estimation for stable training.
- Includes protections against training instabilities.

## 🌟 Why This Model?
- **⚡ Adaptive Thresholds:** Adjusts detection sensitivity in real-time.
- **📉 Crash Hour Analysis:** Focuses on peak volatility during flash crashes.
- **🎯 Custom Reward Structure:** Tackles class imbalance in spoofing detection.
- **🛡️ Resilient Processing:** Built-in error handling and timeout protections.

## 📊 Performance Metrics
We measure success using:
- Precision, recall, and F1 score.
- Confusion matrix analysis.
- Hour-by-hour spoofing pattern identification.
- Anomaly score distributions for in-depth insights.

## 🚀 Getting Started
### Run the Model
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/spoof-detection.git
   cd spoof-detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute the model:
   ```bash
   python main.py --data_path /path/to/data --model_path /path/to/model
   ```

## 📢 Who Should Use This?
This project is perfect for:
- Market surveillance analysts 🕵️
- Flash crash researchers 📉
- AI/ML enthusiasts in finance 🤖
- Traders and regulators ensuring market integrity ⚖️

## 🤝 Contribute
Want to improve the project? Follow these steps:
1. Fork the repo.
2. Create a feature branch (`feature-branch`).
3. Commit your changes.
4. Open a pull request.

## 📜 License
Licensed under MIT. Check `LICENSE` for details.

## 💬 Get in Touch
Have questions or ideas? Open an issue on [GitHub](https://github.com/your-username/spoof-detection/issues) or drop us a message!
