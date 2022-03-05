# Charity Funding Predictor
   **Neural Network Model**
 
![charity-donation-with-sphere-coins_24877-54470](https://user-images.githubusercontent.com/90159408/156863795-abbdd921-692e-4720-a960-ea88a1978f94.jpg)

**Background**

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

**Data Preprocessing**
   
   * Used "IS_SUCCESSFUL as the target for model
   
   * All other columns that were not considered target variables can be used as features except the identification variables
      * CLASSIFICATION AND APPLICATION_TYPE were used for this model
      
   * Removed identification columns ("EIN" and "NAME") from input   
 
 ![Screenshot 2022-03-04 211255](https://user-images.githubusercontent.com/90159408/156863789-c1fe7455-ec19-4a4e-a7c3-957e135cf926.png)

**Compile, Train, and Evaluate the Model**

   * StandardScaler to train and scale model**
   
      
    
   **Defined the model**
   
   ![Screenshot_model](https://user-images.githubusercontent.com/90159408/156864710-f539dbf9-9a59-44b4-9c44-9f581e9146d3.png)R
      
**Results**
      
   *Performance Results (1)*
         
   ![Screenshot_accuracy](https://user-images.githubusercontent.com/90159408/156864730-42ab05b9-4673-489f-bb3b-748f51da06fe.png)

   *Optimized the model to obtain predictive accuracy higher than 75%
      * Dropped "EIN", "SPECIAL column, added more hidden layers and neurons with epochs to the training regimen to receive 79% accuracy*
      
   ![Screenshot_layers](https://user-images.githubusercontent.com/90159408/156865263-a7e00064-b8bf-45dd-a715-891fdf433372.png)

      
   *Performance Results(2)*
   
   ![accuracy2](https://user-images.githubusercontent.com/90159408/156865123-59ce926f-28bb-46ed-a73a-27dbfb8bc16e.png)
            
   Random Forest Results
    
   ![Screenshot_predict](https://user-images.githubusercontent.com/90159408/156865194-bc541578-ba7b-4a4d-bf38-6d9b949ef70f.png)


**Summary** 
Overall results shows the by adding a third layer and using "sigmoid" for second and third layers help reached results to be able to classify 79% of the time. In saying this, it can be determined if the name of the application appears more than five times, has an application type of T3, T4, T6, T5, T19 and a classification of more than 1000, then there's a good (79%) chance of successful funding. 



© 2021  Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.	
