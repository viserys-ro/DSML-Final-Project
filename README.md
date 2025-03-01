# DSML-Final-Project
classification ML
### GitHub README Summary for Room Occupancy Estimation Dataset

#### Dataset Overview
The **Room Occupancy Estimation Dataset** is a publicly available dataset from the **UCI Machine Learning Repository**. It contains sensor data collected from a room to estimate occupancy (whether the room is occupied or not). The dataset is suitable for classification tasks, particularly binary classification, where the goal is to predict room occupancy based on environmental sensor readings.

---

#### Dataset Details
- **Source**: [UCI Machine Learning Repository - Room Occupancy Estimation](https://archive.ics.uci.edu/dataset/864/room+occupancy+estimation)
- **Number of Instances**: 10,130
- **Number of Features**: 7
- **Target Variable**: Binary (Occupancy: 0 = Not Occupied, 1 = Occupied)
- **Features**:
  1. Temperature (in Celsius)
  2. Humidity (in %) 
  3. Light (in Lux)
  4. CO2 (in ppm)
  5. Humidity Ratio (derived from temperature and relative humidity)
  6. Timestamp (optional, can be used for time-series analysis)
- **Missing Values**: None

---

#### Dataset Description
The dataset contains measurements from environmental sensors placed in a room. The goal is to predict whether the room is occupied or not based on the sensor readings. The features include temperature, humidity, light, CO2 levels, and humidity ratio. The target variable is binary, indicating occupancy status.

---

#### Potential Use Cases
1. **Binary Classification**:
   - Predict room occupancy based on sensor data.
   - Algorithms: Logistic Regression, Decision Trees, Random Forest, SVM, etc.

2. **Time-Series Analysis**:
   - Analyze trends in occupancy over time using the timestamp feature.

3. **Feature Importance Analysis**:
   - Determine which sensor readings are most influential in predicting occupancy.

4. **Anomaly Detection**:
   - Detect unusual patterns in sensor data that may indicate errors or unexpected events.

---


---

#### How to Use the Dataset
1. **Download the Dataset**:
   - Visit the [UCI Machine Learning Repository link](https://archive.ics.uci.edu/dataset/864/room+occupancy+estimation) to download the dataset.

2. **Load the Dataset**:
   - Use Python libraries like `pandas` to load the dataset:
     ```python
     import pandas as pd
     url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00484/occupancy_data.zip"
     df = pd.read_csv(url)
     ```

3. **Preprocess the Data**:
   - Handle missing values (if any).
   - Encode categorical variables (if applicable).
   - Scale numerical features if necessary.

4. **Train and Evaluate Models**:
   - Split the dataset into training and testing sets.
   - Train classification models (e.g., Logistic Regression, Random Forest).
   - Evaluate model performance using metrics like accuracy, precision, recall, and F1-score.

---



#### Dataset Challenges
1. **Imbalanced Classes**:
   - The dataset may have an imbalance in the target variable (e.g., more "Not Occupied" instances than "Occupied" instances). Techniques like SMOTE or class weighting can be used to address this.

2. **Feature Correlation**:
   - Some features (e.g., temperature and humidity ratio) may be highly correlated. Feature selection or dimensionality reduction techniques (e.g., PCA) can be applied.

3. **Time-Series Nature**:
   - If the timestamp is used, the dataset can be treated as a time-series problem, requiring specialized techniques for analysis.

---


---

#### References
- [UCI Machine Learning Repository - Room Occupancy Estimation](https://archive.ics.uci.edu/dataset/864/room+occupancy+estimation)
- Dua, D. and Graff, C. (2019). UCI Machine Learning Repository. Irvine, CA: University of California, School of Information and Computer Science.

---

