# TradeSentry: PPO-Based Spoof Detection in Algorithmic Trading

## Overview
TradeSentry is a deep reinforcement learning model designed to detect market manipulation through spoofing tactics. It analyzes Level 3 Limit Order Book (LOB) data to identify patterns where traders place and rapidly cancel large orders to create artificial price movements. The system is particularly focused on detecting anomalies during events like the LUNA flash crash of May 2022.

## Technical Approach
### 1. Data Preprocessing
- Handles Level 3 LOB data, extracting temporal patterns and order attributes.
- Implements robust error handling for real-world financial data.

### 2. Feature Engineering
TradeSentry extracts key features for spoofing detection, including:
- Rolling statistics for price and size movements
- Order flow imbalance metrics
- Cancellation ratios
- Time-sensitive features targeting spoofing behavior

### 3. Market Simulation Environment
- Dynamic spoofing threshold adjustment
- Realistic reward mechanisms
- State representation capturing temporal patterns

### 4. PPO Policy Network
- Implements a neural network architecture to process time-series market data
- Outputs spoofing/non-spoofing classifications
- Adapts to changing market conditions dynamically

### 5. Training & Evaluation
- Efficient experience collection for reinforcement learning
- Robust advantage estimation for stable training
- Protection against training instabilities

## Key Features
- **Adaptive Thresholds**: Dynamically adjusts spoofing detection thresholds based on recent anomaly scores.
- **Crash Hour Analysis**: Special emphasis on peak volatility periods during flash crashes.
- **Customized Reward Structure**: Addresses class imbalance in spoofing detection.
- **Resilient Processing**: Includes robust error handling and timeout protections throughout the pipeline.

## Performance Metrics
TradeSentry evaluates detection performance using:
- Precision, recall, and F1 score
- Confusion matrix analysis
- Hour-by-hour spoofing pattern identification
- Anomaly score distributions

## Usage
### Execution Parameters
The main function accepts parameters for:
- Data path configuration
- Pre-trained model loading
- Training time limits
- Hyperparameter tuning options

### Output Results
Results are saved as:
- Detected spoofing instances in CSV format
- Trained model weights
- Performance visualizations

## Research Applications
This implementation is particularly useful for:
- Market surveillance research
- Flash crash analysis
- Reinforcement learning in financial applications
- Market integrity studies

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/TradeSentry.git
   cd TradeSentry
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the model:
   ```bash
   python main.py --data_path /path/to/data --model_path /path/to/model
   ```

## Contribution
We welcome contributions! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`feature-branch`).
3. Commit your changes.
4. Open a pull request.

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

## Contact
For questions or collaboration opportunities, please reach out via [GitHub Issues](https://github.com/your-username/TradeSentry/issues).
