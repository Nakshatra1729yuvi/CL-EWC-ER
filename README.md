# CL-EWC-ER 🧠🔁
**A combination of Elastic Weight Consolidation and Experience Replay for Continual Learning**

## Overview ✨
This repository implements **Elastic Weight Consolidation (EWC)** and **Experience Replay (ER)** techniques to tackle catastrophic forgetting in continual learning scenarios. By combining EWC's regularization approach with ER's memory buffer strategy, the project aims to achieve efficient knowledge retention when learning multiple tasks sequentially.

## Features 🚀
- **Elastic Weight Consolidation**: Prevents the forgetting of previous tasks by regularizing important network parameters.
- **Experience Replay**: Randomly samples previous experiences to avoid overfitting and reinforce learning.
- **Modular Notebook (`CL_EWC_and_ER.ipynb`)**: Explore, experiment, and reproduce results easily.

## File Structure 📂
- `CL_EWC_and_ER.ipynb` – Main implementation notebook
- `LICENSE` – MIT License

## Usage 💾
1. Clone the repository:
    ```bash
    git clone https://github.com/Nakshatra1729yuvi/CL-EWC-ER.git
    ```
2. Open and run `CL_EWC_and_ER.ipynb` in Jupyter/Colab.
3. Experiment with different datasets, hyperparameters, and model architectures.

## Installation 🛠️
- Python 3.8+
- Required packages (install via pip):
    ```bash
    pip install numpy torch matplotlib
    ```

## Results 📊

**Final Validation Accuracies:**
- After Task 1 (MNIST): **97.76%**
- After Task 2 (FashionMNIST with EWC&ER): **87.29%**
- MNIST (after FashionMNIST + EWC&ER): **92.86%**

**Configuration Parameters:**
- Batch size: 512
- Model: SimpleCNN (dim=768, out_feat=10)
- Optimizer: Adam (lr=1e-3)
- Loss: CrossEntropyLoss
- EWC Lambda: 5000
- Memory size (ER): 10,000
- Epochs per task: 2

## Citation 🎓
If you use this repository in your research, please cite accordingly:
```plaintext
@misc{CL-EWC-ER,
  author = {Nakshatra1729yuvi},
  title = {CL-EWC-ER: A combination of Elastic Weight Consolidation and Experience Replay},
  year = {2025},
  url = {https://github.com/Nakshatra1729yuvi/CL-EWC-ER}
}
```

## License 📄
MIT License
