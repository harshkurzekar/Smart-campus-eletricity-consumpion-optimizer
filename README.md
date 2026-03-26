# Smart-campus-eletricity-consumpion-optimizer

🎓 Campus Energy Optimizer (CEO)
A Machine Learning Approach to Smart Building Management
📌 Project Overview
The Campus Energy Optimizer is a predictive maintenance and automation tool designed to reduce electricity wastage in university environments. By analyzing environmental data (Temperature, Light, CO2, Humidity), this Python-based ML model predicts room occupancy to automate lighting and HVAC systems.

🛠️ Features
 * Real-time Prediction: Classifies room status as Occupied or Vacant.
 * Data-Driven Insights: Visualizes which factors (like CO2 levels) most strongly indicate human presence.
 * Scalable Architecture: Built with modular Python scripts for easy integration with IoT hardware like Raspberry Pi.
📊 The ML Fundamentals Used
 * Exploratory Data Analysis (EDA): Using Seaborn to find correlations between light levels and occupancy.
 * Feature Scaling: Normalizing sensor data so that high CO2 values don't "overpower" humidity values in the model.
 * Binary Classification: Implementing a Random Forest Classifier to handle non-linear relationships in sensor data.
 * Model Evaluation: Using Precision, Recall, and F1-Score instead of just accuracy to ensure no energy-saving opportunities are missed.
🚀 Getting Started
1. Prerequisites
Ensure you have Python 3.8+ installed. You will need the following libraries:
pip install pandas scikit-learn matplotlib seaborn

2. Installation
Clone this repository to your local machine:
git clone https://github.com/your-username/campus-energy-optimizer.git
cd campus-energy-optimizer

3. Running the Model
To train the model and see the results, run:
python src/train_model.py

📂 Repository Structure
 * data/: Contains occupancy_data.csv.
 * notebooks/: EDA.ipynb (Initial data visualization).
 * src/:
   * preprocess.py: Handles data cleaning and scaling.
   * train_model.py: The core ML training script.
 * Report.pdf: Detailed project documentation.
📝 Reflective Summary
This project taught me that data cleaning is 80% of the work in AI. Initially, my model was inaccurate because it didn't account for "Light" fluctuations during sunset. By engineering a "Time of Day" feature, I improved the F1-score by 15%.
📩 Submission Details
 * Author: [Haarsh kurzekar]
 * Course: Python & AI/ML Fundamentals
 * Platform: VITyarthi
