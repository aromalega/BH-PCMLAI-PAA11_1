Problem Statement: Using the CRISP-DM overview, identify the key drivers for used car prices.

Data : I have used the dataset which contains features of 426K used cars.

CRISP-DM Framework

  Business Understanding: Given the features of used cars, find the factors that have highest impact on price of a used car.
  
  Data Understanding: The dataset consists of different features of used cars along with their prices.
  
  Data Preparation: Concerted or removed the data with null values. Used One Hot Encoding on categorical columns to prepare the datset for modeling. Split the data into test and train datasets.
  
  Modeling: Found the mean squared error and key features driving the car prices using the below 3 models.
              Linear Regression
              ![image](https://github.com/user-attachments/assets/27883f9d-8062-43c3-aeff-abd7f695e3bf)

              Ridge Regression
              ![image](https://github.com/user-attachments/assets/3cf2fc7f-83d1-4be2-ad32-3ac3f3216805)

              Lasso Regression
              ![image](https://github.com/user-attachments/assets/bb988604-cdda-4d6c-8f58-e5212739008b)


  Evaluation: Compared the Mean squared errors of 3 models and found the best model for this dataset.
  ![image](https://github.com/user-attachments/assets/3a5f0be9-b48e-4c48-8890-87d435a66c71)

  Since we found the Ridge regression to be the best model, plotted the key features from that model against price to evaluate what in those features contributes to high price.
  ![image](https://github.com/user-attachments/assets/a65392cc-eb0e-413a-97cd-2f367c144317)
  ![image](https://github.com/user-attachments/assets/10ee04e0-d6b9-4a32-914d-01d13bed64c8)
  ![image](https://github.com/user-attachments/assets/2c95a3c5-8f1f-470e-8763-d594894da03e)
  ![image](https://github.com/user-attachments/assets/1e18f07b-b554-4f19-bb30-6f891433d263)

    Deployment: So according to ridge regression, the key drivers for the used car prices are as follows
      cylinders - 8 & 6 cylinders has the highest price
      drive - 4wd & rwd had the high pricing in order
      title_status - cleans title cars have better pricing
      odometer - low odometer has high price
    A used car dealer would need to prioritize the above factors.

    Next Steps: I had to filter down the dataset to only California due to processing Issues. I could further use models on the complete dataset and find more variables that might affect the price.
    




