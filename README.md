# ChemicalCompoundClassification
## ANN model for pedicting Chemical Compound Class
### Pre-processing
The first three columns ID, molecule_name, conformation_name have been ignored as the information contained in the first column is only the index and the other two columns contain the name of the compound.

The data was split into training set and test set in the ratio 80:20.

The StandardScaler from sklearn was used to scale the data.
Variables that are measured at different scales do not contribute equally to the model fitting & model learned function and might end up creating a bias. Thus, to deal with this potential problem feature-wise standardized (μ=0, σ=1) is usually used prior to model fitting.
### Performance
#### Precision:  0.99773
#### Recall:        0.99772
#### F-Score:     0.99772 
### Why ANN?
1. ANNs have the ability to learn and model non-linear and complex relationships, which is really important because the relationships between inputs and outputs are non-linear as well as complex.
2. ANNs can generalize — After learning from the initial inputs and their relationships, it can infer unseen relationships on unseen data as well, thus making the model generalize and predict on unseen data.
3. Unlike many other prediction techniques, ANN does not impose any restrictions on the input variables (like how they should be distributed). 
