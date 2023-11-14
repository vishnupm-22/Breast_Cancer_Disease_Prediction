## **BREAST CANCER CLASSIFICATION**
**Problem Statement**:
* Develop a simple neural network model to detect the breast cancer by classifying the tumor as Malignant/Benign.

**Steps** :
* Understanding the data
* EDA
* Feature Engineering
* Model Building and Evaluation

Used built-in sklearn dataset ('load_breast_cancer()').This dataset contains 31 features such as mean radius, mean texture, mean smoothness, etc., computed from images of breast masses. The target variable 'label' indicates whether the tumor is malignant (1) or benign (0).

**Did exploratory data analysis to gain some insights on data**:
 * **Target Distribution** : plotted bar and pie plot to show number of Malignant and Benign cases.
 * **Feature Distribution** : Plotted dist plot which helps to identify the important features  where the distributions for the two classes have minimal overlap.
 * **Correlation Analysis**: plotted heat map to show that many features are higly correlated which indicates multicollinearity
 * **Outlier Detection** : Detected Outliers using box plot. 

**Feature Engineering**:
 * Handled  outliers using Winsorization method & visualized distribution of the original data with the Winsorized data.
 * Normalization of data before applying PCA. Applied PCA technique to address the issue of multicollinearity.
 * Choosen optimal no_pca_components @  95 % or 99 % cumm_explained_variance by plotting graph between no_pca_components vs cumm_explained_variance .

**Model Building and Evaluation**:
 * Created a Multi Layer Perceptron(MLP) using tensor flow and keras.
 * The MLP model is defined using Sequential from Keras, with three dense layers (i/p ,hidden & o/p layers)
 * The model is compiled with an optimizer (Adam), a loss function (categorical_crossentropy for binary-class classification), and a performance metric (accuracy).
 * Trained and compiled the NN model and visualized model metrics (accuracy and loss) through 30 epochs which performed with an test_validation_accuracy : 0.9783 and test_validation_loss: 0.0802.





  

