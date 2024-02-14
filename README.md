# A_Deep_Learning_Approach_for_Nonprofit_Funding_Selection

Overview

The aim of this project is to develop a deep learning model to assist Alphabet Soup, a nonprofit foundation, in selecting funding applicants with the highest likelihood of success in their ventures. By leveraging machine learning techniques, particularly neural networks, we seek to create a binary classifier capable of predicting whether organizations funded by Alphabet Soup will be successful.

Instructions

Step 1: Data preparation
* Read the charity_data.csv to a Pandas DataFrame.
* Identify target and feature variables
* Drop unnecessary columns (EIN and NAME).
* Determine unique values for each column.
* Bin rare categorical variables.
* Encode categorical variables.
* Split data into features and target arrays.
* Scale the datasets using StandardScaler.

Step 2: Compile, Train, and Evaluate the Model
* Design a neural network model using TensorFlow and Keras.
* Create hidden layers with appropriate activation functions.
* Check the structure of the model.
* Compile and train the model.
* Evaluate model performance using test data.
* Results saved as AlphabetSoupCharity.h5.

Step 3: Optimize the Model
* Adding back "NAME" column and group counts less then 100 into "other"
* With modification the model achieve >75% accuracy.
* Results saved as AlphabetSoupCharity_Optimization.h5.

Step 4: Neural Network Model Findings
* Provide an overview of the analysis.
* Discuss data preprocessing: target(s), feature(s), and unnecessary variables.
* Describe neural network architecture and optimization steps.
* Evaluate model performance and provide recommendations.

Conclusion

This project underscores the critical role of feature selection in enhancing machine learning model accuracy. Despite initial efforts to streamline analysis by reducing the number of features, achieving an accuracy of over 75% necessitated the inclusion of additional layers in the neural network architecture.

Moreover, the reintroduction of the NAME column, with values grouped into an "other" category for occurrences less than 100, notably enhanced model performance. This demonstrates that fewer features do not necessarily translate to improved accuracy. Rather, deliberate feature engineering and selection are pivotal in optimizing model efficacy.

It's noteworthy that too many branches in hidden layers can adversely affect prediction accuracy. Sometimes, an excessive number of branches can even deteriorate model performance. Hence, striking the right balance between complexity and simplicity in neural network architecture is crucial for achieving optimal results.

Ultimately, this project aims to equip Alphabet Soup with the tools to make more informed decisions regarding funding applicants. By developing and refining a robust neural network model, we strive to bolster the foundation's capacity to select organizations with the highest potential for success in their endeavors.