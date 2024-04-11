# deep-learning-model
# Summary

In this project, we developed a tool aimed at aiding the selection of financial applicants with greater potential for success in their projects. Leveraging neural networks, we created a binary classifier capable of predicting whether applicants would secure funding.
# Findings
## Data Processing
## The target variables of the model is:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special considerations for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

The variables of EIN and SPECIAL_CONSIDERATIONS were droppped.

# Training and Evalutaion:

For model architecture, I designed a neural network comprising two input layers with a total of 22 neurons. ReLU activation function was applied to the input and hidden layers with 21 neurons, while the output layer employed the Sigmoid function with a single neuron. This configuration facilitated effective feature extraction and learning of nonlinear relationships, making it well-suited for binary classification tasks. The model demonstrated an accuracy of 78%.

To enhance predictive performance, I introduced the applicant's name as a feature. Additionally, I preprocessed the data by removing outliers in the "CLASSIFICATION" and "APPLICATION_TYPE" fields, excluding those with unique value counts less than 500. Moreover, outliers in the 'NAME' column with counts less than 5 were also filtered out.

In summary, this project culminated in the development of a valuable tool for identifying financial applicants with a higher likelihood of project success. The neural network-based binary classifier offers insights into the probability of applicants securing funding.

For future classification tasks akin to this one, I recommend considering decision tree-based models such as Random Forest. Random Forest leverages the strength of multiple decision trees and their collective predictions, often yielding robust and interpretable results, which could be advantageous depending on the specific requirements of the problem at hand.