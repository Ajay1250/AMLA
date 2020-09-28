# AMLA
[![Watch the video](https://github.com/ScorpionsHackathon/AMLA/blob/master/Amla.PNG?raw=true)](https://youtu.be/_z03YI1Wvpw)
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

# New Features!

  - Import a HTML file and watch it magically convert to Markdown
  - Drag and drop images (requires your Dropbox account be linked)


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

