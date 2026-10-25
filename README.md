# Machine Learning-Assisted Compiler for Healthcare Application Code Analysis

A Compiler Design Lab project that combines traditional compiler techniques with Machine Learning to analyze healthcare-related application code and identify potential programming errors and risks.

##  Project Overview

Healthcare applications require reliable code because programming errors can affect the correctness of medical software. This project explores how compiler design techniques and machine learning can work together to analyze source code and flag potential issues.

The system performs lexical, syntax, and semantic analysis, followed by healthcare-focused rule checks. A Decision Tree classifier is used to classify potential healthcare-related risks identified during analysis.

The project is implemented in **Python using Jupyter Notebook**, without a separate graphical user interface.

##  Objectives

- Implement the fundamental phases of a compiler.
- Identify lexical, syntax, and semantic errors in source code.
- Apply healthcare-focused rules to detect potentially risky code patterns.
- Integrate a Machine Learning classifier for risk classification.
- Evaluate the implementation using test cases and performance metrics.
- Explore the application of compiler design in healthcare software analysis.

##  Key Features

- **Lexical Analysis:** Identifies tokens such as keywords, identifiers, operators, and symbols.
- **Syntax Analysis:** Checks whether source code follows the supported grammar.
- **Semantic Analysis:** Detects issues such as undeclared variables, duplicate declarations, and type mismatches.
- **Healthcare Rule Checks:** Flags selected patterns involving dosage values and other healthcare-related conditions.
- **Machine Learning Classification:** Uses a Decision Tree model to classify potential risk descriptions.
- **Testing and Evaluation:** Includes functional tests, prediction results, evaluation metrics, and visualizations.
- **Result Export:** Saves selected analysis and evaluation results as CSV and JSON files.

##  Technologies Used

- Python
- Jupyter Notebook
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

##  System Workflow

1. Load and preprocess source code.
2. Perform lexical analysis.
3. Perform syntax analysis.
4. Conduct semantic analysis.
5. Apply healthcare-specific rule checks.
6. Classify selected findings using the trained Decision Tree model.
7. Display analysis results and evaluation metrics.
8. Export results for further examination.

##  Project Structure

```text
Healthcare-ML-Assisted-Compiler/
│
├── Healthcare_ML_Assisted_Compiler.ipynb
├── README.md
├── requirements.txt
└── healthcare_compiler_results/
    ├── end_to_end_test_results.csv
    ├── initial_ml_sanity_check.csv
    ├── baseline_ml_evaluation_predictions.csv
    ├── healthcare_risk_predictions.csv
    └── experimental_summary.json
```

*Note: The results folder contains generated outputs. Include it in the repository if you want to publish your experimental results.*

##  Getting Started

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Healthcare-ML-Assisted-Compiler
```

### 2. Install Dependencies

```bash
pip install jupyter pandas numpy scikit-learn matplotlib seaborn
```

### 3. Run the Notebook

```bash
jupyter notebook Healthcare_ML_Assisted_Compiler.ipynb
```

Open the notebook and execute the cells sequentially to run the compiler analysis, healthcare rule checks, machine learning predictions, and evaluation.

##  Testing and Evaluation

The project includes functional tests covering valid declarations, invalid characters, missing semicolons, type mismatches, undeclared variables, duplicate declarations, and healthcare-related warnings.

The healthcare risk classifier was evaluated using a small synthetic dataset, achieving **80% accuracy on a 10-example held-out test set** in the recorded experiment. This result is preliminary and should not be interpreted as evidence of real-world healthcare safety or generalization.

##  Limitations

- The parser supports a limited, C-like subset of source code rather than the complete C programming language.
- The healthcare rules cover selected patterns and cannot identify every possible risk.
- The machine learning model uses synthetic examples and requires evaluation on representative real-world data.
- This project is an educational prototype, not a clinically validated tool. Its output must not be used to determine patient treatment or medication dosage.

##  Future Enhancements

- Expand the supported programming language grammar.
- Add more comprehensive semantic checks and healthcare-specific rules.
- Train and evaluate models using validated, representative datasets.
- Improve error reporting and explainability.
- Integrate static analysis tools for more extensive code verification.

##  Authors

- **S. Mahitha Sree** — 24BCB7023
- **Yarlagadda Rahul** — 24BCB7087

**Institution:** VIT-AP University  
**Program:** B.Tech — Computer Science and Business Systems  
**Project Type:** Compiler Design Lab

##  Disclaimer

This project is developed for academic and educational purposes only. It does not replace professional software verification, clinical validation, or medical expertise.

---

