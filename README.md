# AMLA : Anti Money Laundering Analyzer

Developed By Team Scorpions : Ajay Philip Joy and Michelle Young For Microsoft Encode Hackathon on 27th September 2020
[![Watch the video](https://github.com/aj1250/AMLA/blob/master/pictures/Amla.PNG?raw=true)](https://youtu.be/_z03YI1Wvpw)
Money laundering is the illegal process of making large amounts of money appear to have come from a legitimate source.
The Anti Money Laundering Analyzer (AMLA) is a cloud-based enterprise solution for monitoring, screening and catching suspicious money laundering transactions within the Canadian financial system.
The object of AMLA is to ease the workload of anti-money laundering investigators and analysts by using machine learning techniques to reduce the number of false positive cases that are flagged as money laundering transactions and make sure that no true positive cases are missed out in the bulk


AMLA uses Machine Learning techniques to reduce the number of false positive cases that are detected and reported to FINTRAC.
AMLA also make use of a ranking system so as to priorities each case as required

# FEATURES
  - Allow Users to change the rank of a case
  - Allow Users to review details of each transactions
  - Allow Users to confirm or reject each case as money laundering based on the details reviewed
  - Provide a report to see the perfomance and status of AMLA through a various combinations of visual tiles
  - Provide Various views in which  they can interpret details of various transactions


# Platform USED
  AMLA is a Platform-as-a-Service (PaaS) solution that utilizes the following resources in Azure:
- Azure ML Studio Automated ML
- Azure ML Studio Notebooks
- Azure SQL
- Azure VNet
 - Azure Web APP

# Logic Involved
- AMLA make use of a properly defined flags based on ruleset to filter our and properly detect any transaction which falls under Money Laundering 
- Based on these flags initial filtering of the data is done to form a case and then distinct ranking is provided to each flags.
- Then the daily trained machine learning model is applied on the cases to determine a rank value for that transaction
- The Officer in charge of auditing the case can view the details using the web app and he is given below features
- Can look into details of the account whose transaction is a case and can filter the data based on several factors
- Can approve or reject the case based on his conclusion
- Can bump up or lower the rank if he think it is not a proper value which will be used by ML for training the model in the daily run
- Case will be moved to appropriate category as specified by the officer and a multiple options of views are provided to the officer for an enhanced accessibility

14 sets of Flags were used to efficiently filter out the data to skip non Money Laundering Transactions

# Logical Architecture
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/Logical%20Architectur.png?raw=true)

# Application ScreenShots
    1. Home Page Of the Application
    This Page displays all the cases generated by the solution
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/home.png?raw=true)

    2. Details Page
    This Page displays all the details regarding the cases generated. It will also provide the user with options to update the rank of case , confirm or reject the case and look through various details related to the case
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/details.png?raw=true)

    3. Case Specific to the day Page
    This Page displays all the cases specific to that day
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/dayspecificcase.png?raw=true)

    4. Transactions Specific to the day Page
    This Page list all the transactions which happend on that day
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/dayspecifictrans.png?raw=true)

    5. Officer Confirmed Cases Page
    This Page list all the cases which are confirmed by the officer
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/officerconfirmedcases.png?raw=true)

    6. Officer Rejected Cases Page
    This Page list all the cases which are rejected by the officer
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/officerrejected.png?raw=true)

    7. Report Page
    This Page shows the report which summarize the perfomance and status of AMLA
![alt text](https://github.com/aj1250/AMLA/blob/master/pictures/report.png?raw=true)


Note: This solution was developed for Microsoft Encode Hackathon in a time period of 7 days. So this solution is a proof of concept and not optimized for performance or visual design

