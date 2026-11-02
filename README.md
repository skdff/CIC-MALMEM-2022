# Malware Classification Using Machine Learning Models

Official repository for the source code and experimental framework of the paper published in **Procedia Computer Science**: 
🔗 **[Read the Full Paper on ScienceDirect](https://doi.org/10.1016/j.procs.2024.04.133 "ScienceDirect Paper Link")**

## 📖 Abstract
Malware compromises data integrity and facilitates unauthorized access, causing ongoing internal harm to victim systems until limits are exhausted. To address malware detection challenge, this research evaluates six different machine learning algorithms using a comprehensive pipeline built around the **CIC-MalMem-2022** benchmark dataset. A correlation-based feature selection approach (threshold = 0.6) was used to filter redundant features. Following 10-fold cross-validation, the **Decision Tree** model emerged as the top performer during validation (0.9994240 accuracy), while both **Decision Tree** and **KNN** reached a peak accuracy of **0.9998293** during the testing phase.

## 📊 Methodology Overview

* **Dataset:** [CIC-MalMem-2022 Dataset](https://www.unb.ca/cic/datasets/malmem-2022.html "CIC Dataset Page") containing **29,298 samples** (various malware families and benign instances).
* **Feature Engineering:** Correlation-based Feature Selection (CFS) with a strict threshold value of **0.6**.
* **Validation Strategy:** 10-Fold Cross-Validation.
* **Classifiers Evaluated:**
  * Logistic Regression
  * Support Vector Machine (SVM)
  * K-Nearest Neighbor (KNN)
  * Random Forest
  * Naive Bayes
  * Decision Tree

## 📈 Key Performance Metrics

### 10-Fold Cross-Validation (Best Model: Decision Tree)

| Metric | Value |
| :--- | :--- |
| **Accuracy** | 0.9994240 |
| **Precision** | 0.9996162 |
| **Recall** | 0.9992325 |
| **F1-Score** | 0.9994882 |

### Testing Phase Peak Performance
During final test deployment, **Decision Tree** and **KNN** demonstrated matching top-tier efficiency:
* **Testing Accuracy:** **0.9998293**

---

## 🛠️ Getting Started & Installation

### Prerequisites
Ensure you have Python installed alongside the following required libraries:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

### Usage
1. Clone this repository:
   ```bash
   git clone https://github.com
   cd YOUR_REPO_NAME
   ```
2. Download the `CIC-MalMem-2022` CSV dataset and place it in the designated data directory.
3. Run the model training pipeline script:
   ```bash
   malware with function.ipynb
   ```

## 📝 Citation

If you utilize this code or research framework in your work, please cite our official paper:

```bibtex
@article{kumar2024malware,
  title={Malware Classification Using Machine Learning Models},
  author={Kumar, Sudesh and Shersingh and Kumar, Siddhant and Verma, Karan},
  journal={Procedia Computer Science},
  volume={235},
  pages={1419--1428},
  year={2024},
  publisher={Elsevier},
  doi={10.1016/j.procs.2024.04.133}
}
```

