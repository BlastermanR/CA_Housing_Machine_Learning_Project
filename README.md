### Model Evaluation Pipeline
This project evaluates multiple machine learning models (Neural Network, Support Vector Regressor, Decision Tree) on a shared dataset using common regression metrics (MSE, MAPE, R²). The workflow includes preprocessing data, training models, saving results, and generating comparative plots.

🔧 How to Run the Program
1. Run Preprocessing Script
This step analyzes, cleans, and prepares the original dataset for model input. After running this script: 
Original and processed datasets will be stored in the dataset/ folder.

2. Run Each Model Script
Each model has its own script for training, evaluating, and saving results. These scripts read the processed dataset and write metrics (MSE, MAPE, R²) to CSVs in the results/ folder.

NOTE: Neural Network should take ~ 1/2 Hours, SVR about ~45 Minutes, and Decision Tree a couple seconds

3. Run Postprocessing Script to Generate Comparison Charts
This script reads all model results from the results/ folder, aligns the data, and creates comparative boxplots and violin plots of model performance for each error metric.