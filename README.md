# Charity Funding Predictor -- Neural Network Model Report
![charity-donation-with-sphere-coins_24877-54470](https://user-images.githubusercontent.com/90159408/156863795-abbdd921-692e-4720-a960-ea88a1978f94.jpg)

## Background

The non-profit foundation Alphabet Soup wants to create an algorithm to predict whether or not applicants for funding will be successful. Using machine learning and neural networks, the features provided dataset will be used to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Below are the following columns for the Alphabet Soup dataset:

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively

## Data Preprocessing
   
   * Used "IS_SUCCESSFUL as the target for model
   * All other columns that were not considered target variables can be used as features except the identification variables
      * CLASSIFICATION AND APPLICATION_TYPE were used for this model
   * Removed identification columns ("EIN" and "NAME") from input   
 
 ![Screenshot 2022-03-04 211255](https://user-images.githubusercontent.com/90159408/156863789-c1fe7455-ec19-4a4e-a7c3-957e135cf926.png)

## Compile, Train, and Evaluate the Model
   * Completed StandardScaler
   * Defined the model
      ![Screenshot_model](https://user-images.githubusercontent.com/90159408/156864710-f539dbf9-9a59-44b4-9c44-9f581e9146d3.png)
   * Performance Results (1)
     * ![Screenshot_accuracy](https://user-images.githubusercontent.com/90159408/156864730-42ab05b9-4673-489f-bb3b-748f51da06fe.png)

   * Optimized the model to obtain predictive accuracy higher than 75%
      * Only dropped "EIN" column, added more hidden layers and fewer epochs
      
      
      * Performance Results(2)
            * ![accuracy2](https://user-images.githubusercontent.com/90159408/156865123-59ce926f-28bb-46ed-a73a-27dbfb8bc16e.png)
    * Random Forest Results
            * ![Screenshot_predict](https://user-images.githubusercontent.com/90159408/156865194-bc541578-ba7b-4a4d-bf38-6d9b949ef70f.png)



2. **Results**:






### Step 3: Optimize the Model

Using your knowledge of TensorFlow, optimize your model in order to achieve a target predictive accuracy higher than 75%. If you can't achieve an accuracy higher than 75%, you'll need to make at least three attempts to do so.

Optimize your model in order to achieve a target predictive accuracy higher than 75% by using any or all of the following:

* Adjusting the input data to ensure that there are no variables or outliers that are causing confusion in the model, such as:
  * Dropping more or fewer columns.
  * Creating more bins for rare occurrences in columns.
  * Increasing or decreasing the number of values for each bin.
* Adding more neurons to a hidden layer.
* Adding more hidden layers.
* Using different activation functions for the hidden layers.
* Adding or reducing the number of epochs to the training regimen.

**NOTE**: You will not lose points if your model does not achieve target performance, as long as you make three attempts at optimizing the model in your jupyter notebook.

1. Create a new Jupyter Notebook file and name it `AlphabetSoupCharity_Optimzation.ipynb`.
2. Import your dependencies, and read in the `charity_data.csv` to a Pandas DataFrame.
3. Preprocess the dataset like you did in Step 1, taking into account any modifications to optimize the model.
4. Design a neural network model, taking into account any modifications that will optimize the model to achieve higher than 75% accuracy.
5. Save and export your results to an HDF5 file, and name it `AlphabetSoupCharity_Optimization.h5`.



3. **Summary**: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

- - -

## Rubric

[Unit 21 - Deep Learning Homework Rubric - Charity Funding Predictor](https://docs.google.com/document/d/1SLOROX0lqZwa1ms-iRbHMQr1QSsMT2k0boO9YpFBnHA/edit?usp=sharing)

___
© 2021  Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.	
