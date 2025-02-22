# Generalized RBF for Mining Symbolic Data

## Overview
This repository explores the power of **Radial Basis Functions (RBFs) as universal approximators**, demonstrating their effectiveness in mining symbolic data. The code provides implementations of generalized RBF networks for function approximation, regression, and pattern recognition tasks.

RBFs have been widely recognized for their ability to approximate complex functions with a simple architecture, making them useful in various applications, including **symbolic data mining, time-series forecasting, and classification**.

## Key Features
- **Generalized RBF Implementation**: Extends traditional RBF networks for enhanced function approximation.
- **Universal Approximation Capability**: Demonstrates how RBFs can approximate arbitrary functions given sufficient neurons.
- **GPU Acceleration (Planned)**: A future goal is to optimize the implementation using CUDA for faster training.
- **Comparison with Alternative Methods**: Benchmarking against Gaussian Process Regression (GPR) and other models.

## Repository Structure
```
GeneralizedRBF_miningSymbolicData/
│── data/                  # Sample datasets for testing RBF networks
│── models/                # RBF model implementations
│── notebooks/             # Jupyter notebooks with experiments
│── scripts/               # Standalone Python scripts for running models
│── tests/                 # Unit tests for validation
│── results/               # Saved results and performance metrics
│── README.md              # This file
│── requirements.txt       # Dependencies
```

## Installation
Clone the repository and install the required dependencies:
```sh
git clone https://github.com/vliviu/GeneralizedRBF_miningSymbolicData.git
cd GeneralizedRBF_miningSymbolicData
pip install -r requirements.txt
```

## Usage
Run the RBF training script on sample data:
```sh
python scripts/train_rbf.py --dataset data/sample.csv --epochs 100 --lr 0.01
```
Or use the Jupyter notebooks for interactive experiments:
```sh
jupyter notebook notebooks/RBF_approximation.ipynb
```

## Results
The experiments demonstrate that **RBFs achieve low error rates in function approximation**, reinforcing their theoretical **universal approximation property**. A comparison with Gaussian Process Regression (GPR) reveals that RBFs provide competitive performance while being more scalable in certain cases.

## Future Work
- **GPU-accelerated RBF implementation** for faster training using PyTorch.
- **Hybrid approaches** combining RBFs with deep learning for enhanced performance.
- **Real-world applications** on symbolic and structured data.

## References
- Broomhead, D. S., & Lowe, D. (1988). **Radial Basis Functions, Multi-variable Functional Interpolation and Adaptive Networks**.
- Park, J., & Sandberg, I. W. (1991). **Universal Approximation Using Radial-Basis-Function Networks**.
- S. Papadimitriou, L. Vladutu et. al (2002) ** Generalized Radial Basis Function Networks Trained with Instance Based Learning for Data Mining of Symbolic Data**, Applied Intelligence 16, 223–234, Kluwer.

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to enhance the repository.

## License
MIT License. See [LICENSE](LICENSE) for details.

