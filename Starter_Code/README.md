FOR IMAGES PLEASE REVIEW DOC FILE (DEEP LEARNING REPORT)

overview:
The purpose of this program is to create a tool for the nonprofit foundation Alphabet Soup that can help it select the applicants for funding with the best chance of success in their ventures. 

Results:
What variables are the targets?
•	IS_SUCCESSFUL

What variable(s) are the features for your model?
•	APPLICATION_TYPE
•	AFFILIATION
•	CLASSIFICATION
•	USE_CASE
•	ORGANIZATION
•	STATUS
•	INCOME_AMT
•	SPECIAL_CONSIDERATIONS

What variable(s) should be removed from the input data because they are neither targets nor features?
•	ASK_AMT

Compiling, Training, and Evaluating the Model:
How many neurons, layers, and activation functions did you select for your neural network model, and why?
 
Due to the amount of features we required at least the first layer to have 43 neurons to process all the data.
We have 2 hidden layers to process all the information from the first layer and the output layer with 1 neuron
Were you able to achieve the target model performance? No
What steps did you take in your attempts to increase model performance? 
I used tensorflow and in different files tried to do the following
•	Remove features
•	Add more hidden layers
•	Add neurons
•	Increase epochs
 

Summary
Using tensorflow tuner, the best result that was achieved showed an accuracy of 73.67%

Here are the best parameters achieved
{'activation': 'sigmoid', 'first_units': 100, 'num_layers': 5, 'units_0': 100, 'units_1': 15, 'units_2': 90, 'units_3': 30, 'units_4': 85, 'units_5': 15, 'tuner/epochs': 50, 'tuner/initial_epoch': 0, 'tuner/bracket': 0, 'tuner/round': 0}
{'activation': 'sigmoid', 'first_units': 65, 'num_layers': 3, 'units_0': 35, 'units_1': 10, 'units_2': 25, 'units_3': 85, 'units_4': 95, 'units_5': 45, 'tuner/epochs': 50, 'tuner/initial_epoch': 0, 'tuner/bracket': 0, 'tuner/round': 0}
