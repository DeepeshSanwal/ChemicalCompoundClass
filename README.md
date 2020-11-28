# ChemicalCompoundClassification
## ANN model for pedicting Chemical Compound Class
### Libraries Used
NumPy
MatplotLib
TensorFlow
### Pre-processing
The first three columns ID, molecule_name, conformation_name have been ignored as the information contained in the first column is only the index and the other two columns contain the name of the compound.

The data was split into training set and test set in the ratio 80:20.

The StandardScaler from sklearn was used to scale the data.
Variables that are measured at different scales do not contribute equally to the model fitting & model learned function and might end up creating a bias. Thus, to deal with this potential problem feature-wise standardized (μ=0, σ=1) is usually used prior to model fitting.
### Building ANN Model
We are using Keras for constructing a neural network. In this model, we are using an input layer of 6 values and an output layer of 1 value since we only want to know binary prediction of 0/1.

Also, we are using two hidden layers of 6 dimension. The output layer takes different activation function and for the case of binary classification, it is sigmoid.

Here loss is cross entropy loss. binary_crossentropy specifies that we have only two classes. The optimizer is Adam. Metrics which is used to specify the way we want to judge the performance of our neural network - accuracy.
### Current Performance Measures
#### Precision:  0.99773
#### Recall:        0.99772
#### F-Score:     0.99772 
