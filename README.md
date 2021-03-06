# PhishDetect
> Be **Aware** Be **Secured** Be **Safe**

## Overview of the project
Phishing is a type of social engineering attack often used to steal user data, including login credentials and credit card numbers. It occurs when an attacker, masquerading as a trusted entity, dupes a victim into opening an email, instant message, or text message. The recipient is then tricked into clicking a malicious link.
Phishing is one of the luring techniques used by phishing artist in the intention of exploiting the personal details of unsuspected users. Phishing website is a mock website that looks similar in appearance but different in destination. The unsuspected users post their data thinking that these websites come from trusted financial institutions. Several antiphishing techniques emerge continuously but phishers come with new technique by breaking all the antiphishing mechanisms. Hence there is a need for efficient mechanism for the prediction of phishing website.

## Data Collection

The set of phishing URLs are collected from opensource service called  **PhishTank**. To download the data:  [https://www.phishtank.com/developer_info.php](https://www.phishtank.com/developer_info.php). From this dataset, 5000 random phishing URLs are collected to train the Machine Learning models.

## Feature Extraction
The below mentioned category of features are extracted from the URL data:

* Address Bar based Features\
          In this category 9 features are extracted.\
          1.Domain of the URL\
          2.HavingIP\
          3.HaveAtSign\
          4.GetLength\
          5.GetDepth\
          6.Redirection\
          7.HttpDomain\
          8.Shortening services\
          9.PrefixSuffix
* Domain based Features\
          In this category 4 features are extracted.\
          1.DNS Record\
          2.Website Traffic\ 
          3.Age of Domain\
          4.End Period of Domain
* HTML & Javascript based Features\
          In this category 4 features are extracted.\
          1.IFrame Redirection\
          2.Status Bar Customization\
          3.Disabling Right Click\
          4.Website Forwarding

The details to extract these features are mentioned in the URL Feature Extraction.ipynb

## Models Used

* Decision Tree
* Random Forest
* XGBoost
* Support Vector Machines

## Installation and Steps to run the code.

Install the requirements.txt by using the commands given below:\
    1. Open cmd from location where code is stored.\
    2. Enter the command pip install -r requirements.txt\
    3. Then all the required libraries are installed.\
    4. Run the code app.py
    
For running as docker :\
    1.Install Docker.\
    2.run docker build . -t name for image\
    3.run docker images (copy the imageid of the respective project)\
    4.run docker run -it -p 5000:5000 image id
          
## Screenshots

![Capture](https://user-images.githubusercontent.com/53186985/155356710-8b0c32ab-aa66-409e-a308-6b6b85f11c76.PNG)

![as](https://user-images.githubusercontent.com/53186985/155380184-9d1f84b5-a1b2-4099-a37a-9a7f5137210a.PNG)

## 

> This project is done by Students of Keshav Memorial Institute of Technology as Mini Project.

