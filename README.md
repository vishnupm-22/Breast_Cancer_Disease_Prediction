
## **BREAST CANCER CLASSIFICATION**
**problem statement**:
* Develop a simple neural network model to detect the breast cancer by classifying the tumor as Malignant/Benign.

**Steps** :
* Understanding the data
* EDA
* Feature Extraction
* Model Building and Evaluation
* Building a predictive system

**Did exploratory data analysis to gain some insights on data**:
 * **Target Distribution** : plotted bar and pie plot to show number of Malignant and Benign cases.
 * **Correlation Analysis**: plotted heat map to show that many features are higly correlated which indicates multicollinearity
 * **Feature Distribution** : Plotted dist plot which helps to identify the feature  where the distributions for the two classes have minimal overlap.
 * **Outlier Detection** : Detecting Outliers using box plot , handled these outliers using Winsorization method & Visualized distribution of the original data with the Winsorized data.

**Feature Extraction**:
 * Applied PCA technique to address the issue of multicollinearity
 * By plotting graph between no_pca_components vs cumm_explained_variance , choosen no_pca_components @ cumm_explained_variance 95 % or 99 %

**Model Building and Evaluation**:
 * Created a MLP using tensor flow and keras.
 * The MLP model is defined using Sequential from Keras, with three dense layers (i/p ,hidden & o/p layers)
 * The model is compiled with an optimizer (Adam), a loss function (categorical_crossentropy for multi-class classification), and a performance metric (accuracy).
 * Trained and compiled the NN model and visualized model metrics (accuracy and loss) through 30 epochs which performed with an validation_accuracy of 0.9783 and val_loss: 0.0802

  

