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

This project underscores the importance of feature selection in machine learning model accuracy. Initially, we attempted to streamline the analysis by removing both the EIN and NAME columns to reduce the number of features. However, even with the reduction in features, achieving an accuracy of over 75% required the incorporation of additional layers in the neural network architecture.

Surprisingly, reintroducing the NAME column, grouped by values with occurrences less than 100 into an "other" category, significantly improved model performance. This highlights the notion that fewer features do not necessarily equate to higher accuracy. Instead, thoughtful feature engineering and selection play a crucial role in model efficacy.

Ultimately, the project aims to empower Alphabet Soup in making more informed decisions regarding funding applicants. Through the development and optimization of a robust neural network model, we aspire to enhance the foundation's ability to select organizations with the highest likelihood of success in their endeavors.