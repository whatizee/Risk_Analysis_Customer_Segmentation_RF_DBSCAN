

# Motor Insurance Risk Analysis using Random Forest and DBSCAN

This project focuses on analyzing motor insurance data to predict customer risk levels using a **Random Forest Classifier** and segment customers using **DBSCAN**. The goal is to improve risk assessment accuracy and identify high-risk customer segments for better decision-making.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Features](#features)
4. [Implementation](#implementation)
   - [Random Forest Classifier](#random-forest-classifier)
   - [DBSCAN Clustering](#dbscan-clustering)
5. [Results](#results)
6. [Dependencies](#dependencies)
7. [How to Run](#how-to-run)
8. [License](#license)

---

## Project Overview
The project addresses inconsistent risk assessments in motor insurance by:
1. **Predicting Risk Levels**: Using a Random Forest Classifier to predict customer risk levels (Low, Moderate, High, Very High).
2. **Customer Segmentation**: Using DBSCAN to segment customers based on their features for better understanding and targeting.

---

## Dataset
The dataset used in this project is synthetic and contains **7343 rows** with the following features:
- **Driver Demographics**: Age, Gender, Occupation
- **Driving History**: Years Driving, Claims Frequency, Claim Severity, Traffic Violations
- **Vehicle Information**: Vehicle Age, Vehicle Type
- **Usage Patterns**: Annual Mileage, Location (Urban/Rural)
- **Target Variable**: Risk Level (Low, Moderate, High, Very High)

The dataset is stored in `motor_insurance_data.csv`.

---

## Features
### Input Features
- Numeric Features: Age, Years Driving, Annual Mileage, Claims Frequency, Claim Severity, Traffic Violations, Vehicle Age
- Categorical Features: Gender, Occupation, Vehicle Type, Location

### Target Variable
- Risk Level: Low, Moderate, High, Very High

---

## Implementation
### Random Forest Classifier
- Used for predicting customer risk levels.
- Includes cross-validation and feature importance analysis.
- Achieves high accuracy in risk prediction.

### DBSCAN Clustering
- Used for customer segmentation.
- Identifies natural clusters in the data based on customer features.
- Helps in understanding customer behavior and risk profiles.

---

## Results
1. **Random Forest Classifier**:
   - Cross-validation accuracy: ~92%
   - Test accuracy: ~91%
   - Top 7 features by importance:
     1. Claims Frequency
     2. Claim Severity
     3. Annual Mileage
     4. Traffic Violations
     5. Vehicle Age
     6. Years Driving
     7. Age

2. **DBSCAN Clustering**:
   - Number of clusters identified: 4
   - Visualized using a scatter plot of Annual Mileage vs. Claims Frequency.

---

## Dependencies
To run this project, you need the following Python libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Install the dependencies using:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/motor-insurance-analysis.git
   cd motor-insurance-analysis
   ```

2. Generate the synthetic dataset (if not already available):
   ```bash
   python generate_data.py
   ```

3. Run the analysis:
   ```bash
   python main.py
   ```

4. View the results:
   - Risk prediction accuracy and feature importance are printed in the console.
   - Customer segmentation plots are saved as `segmentation_plot.png`.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Author
Jibin Sebastian

---

```


