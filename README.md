# Features Selection Project

## Overview
This project explores advanced feature selection techniques to enhance model performance on the "Breast Cancer Wisconsin (Diagnostic)" dataset. It employs various methods, including the Bidirectional Search (BDS) method, Mutual Information Feature Selection (MIFS), Variance, and Correlation methods, to identify the most significant features for accurate predictions.

## Components

### Python Scripts
- **`mathFunctions.py`**: Implements mathematical operations and algorithms for feature analysis.
- **`metrics.py`**: Provides metrics for model performance evaluation.
- **`printScore.py`**: Displays and logs performance metrics.
- **`utils.py`**: Utility functions for data preprocessing and auxiliary tasks.

### Jupyter Notebook (`main.ipynb`)
The notebook includes detailed explanations and implementations of several feature selection methods:
- **Discretization with ChiMerge**: Outlines the process of transforming continuous data into discrete bins based on chi-squared statistics.
- **Entropy-Based Methods**: Discusses the principles of Entropy, Joint Entropy, and Conditional Entropy in the context of information gain.
- **Mutual Information Feature Selection (MIFS)**: Utilizes mutual information to evaluate feature relevance, inspired by Roberto Battiti's work in "Using Mutual Information for Selecting Features in Supervised Neural Net Learning", IEEE Transactions on Neural Networks, August 1994. DOI: [10.1109/72.298224](https://doi.org/10.1109/72.298224).
- **Correlation Feature Selection (CFS)**: A filter-based method that evaluates the predictive ability of feature subsets considering redundancy.
- **Sequential Forward Selection (SFS)**: An incremental method that starts with a single attribute and adds attributes to optimize the feature set.
- **Sequential Forward Floating Selection (SFFS)**: Combines elements of forward selection and backward elimination to iteratively refine the feature subset for optimal performance.
- **Variance Method**: Evaluates features based on their variance, with the premise that features with low variance may contain less information.
- **Correlation Method**: Assesses the strength of the relationship between each feature and the target variable, prioritizing features with high correlation to the target.

## Dataset
Uses the "Breast Cancer Wisconsin (Diagnostic)" dataset, focusing on cell nuclei characteristics from breast mass FNA images.

## Getting Started
To get started with this project, follow these steps:
1. **Environment Setup**: Ensure Python 3.6 or higher is installed on your system. It's recommended to use a virtual environment for Python projects to manage dependencies efficiently.
2. **Clone the Repository**: Download or clone this project repository to your local machine.
3. **Install Dependencies**: Navigate to the project directory in your terminal and run `pip install -r requirements.txt` to install the necessary Python libraries.
4. **Explore the Notebook**: Open the Jupyter Notebook (`main.ipynb`) in your Jupyter environment. You can do this by running `jupyter notebook` or `jupyter lab` in your terminal within the project directory.
5. **Run the Notebook**: Execute the cells in the Jupyter notebook sequentially to understand the feature selection process, methodologies applied, and to view the results.

## Results
The application of various feature selection methods has led to key findings, including the identification of highly informative features and comparisons of method effectiveness. Incorporating selected features into predictive models demonstrated an improvement in performance metrics.

## Conclusion
This project underscores the critical role of feature selection in machine learning workflows. The Mutual Information Feature Selection (MIFS) method, inspired by Roberto Battiti's work, proved especially valuable. Future work could explore more dynamic integration of feature selection with model training and the application of these methods to other datasets.

## References
- Battiti, R. (1994). Using Mutual Information for Selecting Features in Supervised Neural Net Learning. IEEE Transactions on Neural Networks, 5(4), 537-550. DOI: 10.1109/72.298224.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.