# <font color=#10D3F1>Customer Churn Problem: Historical Data Analysis And Predictions</font><br> #
## <a href='#Business-Understanding'>1. Business Understanding</a> ##
## <a href='#Analytical-Approach'>2. Analytical Approach</a> ##
## <a href='#Data-requirements'>3. Data requirements</a> ##
## <a href='#Data-Understanding'>4. Data Understanding</a> ##
## <a href='#Data-Preparation'>5. Data Preparation</a> ##
## <a href='#Modeling'>6. Modeling</a> ##
## <a href='#Evaluation'>7. Evaluation</a> ##
## ====================================================== ##

## <a id='Business-Understanding'>1. Business Understanding</a> ##

Customer churn by definition is the pourcentage of customers (players, subscribers to a service, service users etc.) that ceased their relationship with the company, <br> in other terms, stopped using the provided service/product during a certain time frame. <br>This rate can be calculated from the number of cutomers lost during a time frame divided by the number of the customers at the beginning of the time period.<br>
The full cost of churn when a customers leaves a company includes the lost revenue and the marketing costs involved with replacing him with new a customer which is highly expensive. <br>And this is why a **Churn Analysis** or the evaluation of a company's customer loss rate is order to reduce it is very important and very profitable as it can help minimizing the churn rates.<br>
In this paper we will make an analysis on historical data in order to study the main factors of a company's customer churn, to be able at the end to 
predict whether a client is most likely to stay or leave based on his informations whicn can help take effective measurement (discounts/ oriented promotions/ retention marketing programs) towards specific subset of customers.

## <a id='Analytical-Approach'>2. Analytical Approach</a> ##

We are facing a standard classification problem precicely a binary classification, our model is supposed to predict whether a customer ceases their contract or keeps using the service. In that regard our target variable can take two discrete values **Yes** and **No** in this case.<br> The approach we are taking for this paper is:
- Analyzing the relation between different customer information and how that might effect their departure or stay in the company by defining the target variable to predict (Churn) and the independant variables on which our prediction is based off of (customer informations).
- Sudying key statistical measurements about the relation deduced.

## <a id='Data-requirements'>3. Data requirements</a> ##

In order to achieve this paper's goals, we will use semi structured historical customer data provided from the company.<br>
This data includes general information about the client and the type of service he is benefiting of as well as the interactions between
the customer and company like payment method and contract type and of course our target variable **Churn**.

## <a id='Data-Understanding'>4. Data Understanding</a> ##
The data set in use includes:<br>
**20** Features:<br>
**customerID:** The customer ID<br>
**gender:** Whether the customer is a male or a female<br>
**SeniorCitizen:** Whether the customer is a senior citizen or not (1, 0)<br>
**Partner:** Whether the customer has a partner or not (Yes, No)<br>
**Dependents:** Whether the customer has dependents or not (Yes, No)<br>
**tenure:** Number of months the customer has stayed with the company<br>
**PhoneService:** Whether the customer has a phone service or not (Yes, No)<br>
**MultipleLines:** Whether the customer has multiple lines or not (Yes, No, No phone service)<br>
**InternetService:** Customer’s internet service provider (DSL, Fiber optic, No)<br>
**OnlineSecurity:** Whether the customer has online security or not (Yes, No, No internet service)<br>
**OnlineBackup:** Whether the customer has online backup or not (Yes, No, No internet service)<br>
**DeviceProtection:** Whether the customer has device protection or not (Yes, No, No internet service)<br>
**TechSupport:** Whether the customer has tech support or not (Yes, No, No internet service)<br>
**StreamingTV:** Whether the customer has streaming TV or not (Yes, No, No internet service)<br>
**StreamingMovies:** Whether the customer has streaming movies or not (Yes, No, No internet service)<br>
**Contract:** The contract term of the customer (Month-to-month, One year, Two year)<br>
**PaperlessBilling:** Whether the customer has paperless billing or not (Yes, No)<br>
**PaymentMethod:** The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic))<br>
**MonthlyCharges:** The amount charged to the customer monthly<br>
**TotalCharges:** The total amount charged to the customer<br>
A target variable:<br>
**Churn:** Whether the customer churned or not (Yes or No)
