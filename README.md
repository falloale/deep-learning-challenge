# deep-learning-challenge - Report

## Overview: 
From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. I've used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Data Processing
The dataset removed any irrelevent information; such as, EIN and Name. Both items were dropped from the model. The remaining columns were considered features for the model. NAME was added back in on the second test. CLASSIFICATION and APPLICATION_TYPE were4 both repalced with 'other' due to high fluctuation. The data was then split in two sets, training and testing. The target variable for the model is "IS_SUCCESSFUL" and i verified by the values 1 and 0. 1 was considered 'yes' and 0 was considered 'no'. APPLICATION data was analuyzed and CLASSIFICATION's value was used for binning. Each unique value used several data points as a cutof points to bin "rare" categorical variables together in a new value.'other'. Afterwards we checked to see if binningw as successful.

## Compliling, training and evaluating the model
Neural Netowrk was applied on each model in multiple layers, total of threed. The number of features dictated the number of hidden nodes. 

<img width="981" alt="Screenshot 2023-06-04 at 5 27 53 PM" src="https://github.com/falloale/deep-learning-challenge/assets/119981413/ff1b5d5c-409c-4987-a57d-bbd99a64e96e">
<img width="570" alt="Screenshot 2023-06-04 at 5 30 25 PM" src="https://github.com/falloale/deep-learning-challenge/assets/119981413/36bc2233-4d1b-4281-a91c-e3e3826224bb">

The sequential_1 training model generated 477 parameters. The first attempt had accuracy of 72.6%, with the desired accuracy to be at 75% or higher. 

## Optimization

The second attempt added "NAME" back into the dataset and with the addition we achieved a 78.7% accurary, which is greater than the desired 75%. This also allotted 3,298 parameters compared to the 477 in the first model. 
<img width="570" alt="Screenshot 2023-06-04 at 5 33 26 PM" src="https://github.com/falloale/deep-learning-challenge/assets/119981413/9da31360-3643-4ee1-a2ff-236965a74ecd">
<img width="651" alt="Screenshot 2023-06-04 at 5 35 05 PM" src="https://github.com/falloale/deep-learning-challenge/assets/119981413/bb88a42b-defc-49c3-be10-ff80fadc6e45">


Deep learning models should have multiple layers due to it being machine based. This teaches the computer to filter inputs through the layers to learn how to classify and predict information





