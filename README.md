# // **AI Project 01** //
#### // **Kaggle CareerCon 2019:** Help Navigate Robots

- [Link to Online Competition Here](https://www.kaggle.com/c/career-con-2019/overview)

#### // Student Name: 
- Justin Snider 

#### // Student Number: 
- js10853

#### // Dataset From NYU Faculty:
- y_train_new.csv
- X_train_new.csv
- y_test_new.csv
- X_test_new.csv

#### // File:
- AI_Project_01.ipynb

# // **Conclusions** //
## Settings:
- Epochs: 400
  - If we increase the number the model is over trained. The predictions become very bad for any new data.
  - If we decrease the number the model does not reach the high point of 95% correct predictions.
- Learning Rate: 0.012
  - The learning rate is very important. With a value of 0.012 we are able to get 95% correct predictions. However, anything larger or smaller will peak at a lower correct prediction rate.
  - Using typical values and a neural network with less layers and less nodes we originally had a prediction rate of about 80%. We are able to increase this prediction rate to 95% by optimizing the settings.

## Data:
- Using the original data with no abstracted stats gave a prediction rate of around 50% correct.
- Using instead the stats we abstracted from the raw sequence data boosted our test prediction rate from around 50% up to around 80%.

## Neural Network:
- Much of the neural network is standard based on our number of inputs, type of data, and 9 class mutually exclusive classification output.
- We made a few changes that improved the prediction rate.
  - We increased the number of hidden layers from 1 to 2.
  - We increased the number of nodes on the hidden layers.
- Together with improving the settings (such as learning rate and epoch count) the updated neural network improved prediction rates on the test set from 80% to 95%.
