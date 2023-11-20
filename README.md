### Assignment for UC Berkeley Professional Certificate in Machine Learning and Artificial Intelligence.

**Overview**

The goal of this project is to understand what factors make a car more or less expensive. To accomplish the task, use the standard process in the industry for data projects called **CRISP-DM (Cross-Industry Standard Process for Data Mining)**. This process provides a framework for working through a data problem.
As a result, create a prediction model for used car prices and provide clear recommendations to your client -- a used car dealership -- as to what consumers value in a used car.

**Data**

This dataset comes from Kaggle.The original dataset contained information on 3 million used cars. The provided dataset contains information on 426K cars to ensure speed of processing.
The dataset contains 426880 rows and 18 columns. The data captures the important features of the used cars like year, odometer reading, condition of the car, manufacturer and model of the car etc.. Some of the features have missing values. There are 4 numerical features and 14 non-numeric, also referred as categorical features.

**Deliverables**

After understanding, preparing, and modeling your data, write up a basic report that details your primary findings. Your audience for this report is a group of used car dealers interested in fine-tuning their inventory.

### Final Findings (Includes Technical Terms)
* The data was reviewed, transformed, cleaned and scaled before proceeding with preparation of the model to predict the used vehicle prices.
* Multiple Machine Learning algorithms were tried before arriving at the best model. The best model emerged using the **Random Forest Regression** after tuning the hyper-parameters, that can predict used vehicle prices with **88% accuracy**. 
* **Feature Importance** technique was used to find the important features that were most useful in predicting the target variable (Price). The year of the vehicle is by far the main factor when calculating the price with almost a 44%, followed by the odometer showing importance of ~15%.
* Surprisingly number of cylinders palyed more important role in defining the model compared to manufacturer and model of the cars.
* It seems the region/state also plays a part, which totally makes sense. For example - Specialised cars like sport or convertibles would be a better fit in warmer regions compared to bigger trucks and SUVs that might be more popular in colder places.

### Recommendations to the Used Car Dealers
* Diesels car with 'like new' and 'excellent' conditions are likely to fetch higher price.
* Cars with odometer reading between 0 and 60K miles usually fetch almost double price compared to cars with 90K and above miles.
* Cars with title status other than clean and lien are least preferred by potential buyers.
* Ford-150 is the most sold model among used cars. Ford manufacturer in general is most popular among used car buyers.
* It is recommended to stock the cars according to region/state popularity. For example - certain models might be more popular in Florida (warm state) vs Minnesota (cold state).
* Correct price tag is the key to sell an used car. Mastering the pricing of used cars is not an easy job. Price prediction model can help but it still requires some discretion by the car pricing experts.
* As per current prediction model, the top 5 most important features are:
    * Year **42.26%** 
        * Keep more newer cars in the inventory
    * Odometer **14.55%** 
        * Keep cars with low odometer reading, i.e. less than 60K miles, in the inventory
    * Cylinders **12.68%** 
        * Keep cars with higher number of cylinders, i.e. 6-10 cylinders, in the inventory
    * Fuel Type **6.15%** 
        * Keep more cars with fuel type diesel and electric in the inventory
    * Manufacturer **5.64%** 
        * Keep more cars from popular manufacturer like Ford and Chevrolet in the inventory
* The best model predicted the price of a used car with **88% accuracy**. This information can have an enormous value for both companies and individuals when trying to understand how to estimate the value of a vehicle and, more importantly, the key factors that determine its pricing.

### Next Steps
* There are other predictive models that can be tried to find even a better model.
* The current model can be further tuned to find better hyper-parameters value.
* Data transformation, cleaning (EDA) can be revisited to improve data quality.

**The jupyter notebook can be located in this repository here - https://github.com/jaiomrana/ucb_ai_ml_assignment_11_1/blob/main/used_vehicles_price_model.ipynb**
