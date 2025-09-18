# Drug-Target-Binding-Affinity-Prediction

### All relevant directories and files:

/EC50_bind.tsv.zip: The dataset utilized to train the Supervised_Learning_Model_1_Random_Forest_Regression ML model

/Model_Drug Target Binding Affinity.ipynb: Implementation of a Random Forest Regression model, which utilized the BindingDB_Kd dataset to train. This version of the Random Forest Regressor focused on the Mean Squared Error, R-squared, and Mean Absolute Error metrics. The model was trained with 80% of the dataset and depths of 10, 20, and unspecified

/PCA & Visualize - Supervised_Learning_Model_2_Neural_Network.ipynb: Implementation of a Neural Network model, which utilized the EC50_bind.tsv data file. This implementation of the Neural Network focused on a test split ratio of 0.2 and a batch size of 32. The Neural Network followed the architecture of LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV. The model was then evaluated for Training Loss. This notebook also includes the visualizations for Training Loss vs. Epoch and Confusion Matrix for Regression (Discretized).

/PCA - Supervised_Learning_Model_2_Neural_Network.ipynb: Implementation of a Neural Network model with PCA applied to the dataset, which utilized the EC50_bind.tsv data file. PCA was applied to the drug features with 1000 components, and to the target protein features with 15 components. The Neural Network was then executed with a test split ratio of 0.2 and a batch size of 32. The Neural Network followed the architecture of LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV. The model was then evaluated for Test Loss. This notebook also includes the visualizations for Principal Component Analysis utilized for data pre-processing.

/Pre-processing_Drug Target Binding Affinity.ipynb: Initial data pre-processing, which included transforming of the data to log-scale for stabilization, removal of duplicate pairs of drug molecules and their target proteins, feature generation and aggregation, and normalization of the data.

/Supervised_Learning_Model_1_Random_Forest_Regression.ipynb: Implementation of a Random Forest Regression model, which utilized the EC50_bind.tsv data file. This implementation of the Random Forest Regressor focused on minimizing the Mean Squared Error as a means for measuring the accuracy of the model. The model was trained at various dataset training percentages as well as depths 5, 10, 20, 30 and unspecified. This notebook also includes the data visualizations of our model.

/Supervised_Learning_Model_2_Neural_Network.ipynb: Implementation of a Neural Network model, which utilized the EC50_bind.tsv data file. This implementation of the Neural Network focused on optimizing the loss over several training instances by maintaining state variables between training instances. Each instance was trained with a test split ratio of 0.2 and a batch size of 32. The Neural Network followed the architecture of LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV - RELU - DROPOUT - LINEAR CONV. The model was then evaluated for Test Loss.

/Unsupervised_Learning_Model_1_KMeans.ipynb: Implementation of KMeans clustering model, which utilized the EC50_bind.tsv data file. This implementation focused on varying the combination of data features and the number of clusters per execution. As an unsupervised model, the entire dataset was utilized for clustering, and was then evaluated based on affinity standard deviation. This notebooke also includes visualizations in both 2 and 3 dimensions for each feature and cluster combination.


Authored by: Tamarin Tandra, Pratham Mehta, Elaine Bradley, Chenyu Gu
