# Safeguarding-the-Web
My project titled “Safeguarding the Web: Machine Learning Techniques for Phishing Detection” aims to provide a useful prediction of fraudulent websites. It was the feature extraction in which properties including domain, IP address, use of @ symbol, use of tiny or short URLs, and web traffic data were collected and transformed into a dataset. Using that dataset, the process of machine learning is carried out. The phishing URLs are collected from an open-source service such as PhishTank on the web. This service delivers a combination of phishing URLs in CSV, JSON, and any file format that is updated hourly. Thus, from this dataset, 5000 random samples are extracted. The legitimate URLs are collected from open datasets of the University of Brunswick. This dataset has a collection of benign, spam, phishing, malware and defacement URLs. Out of all these types, the 5000 benign URL datasets are collected for this project to train the ML models on them.

## FEATURE EXTRACTION
Feature extraction is an essential step in the detection process where the characteristics of the URLs are mainly categorized into 3 main groups:
1.	Address Bar based features
2.	Domain-based features
3.	HTML based features 

Address Bar-Based Features
The following features were pulled from the address bar of the given URL:

-	Domain: The first part of the URL which tells the website's legitimacy.
 -	IP address: The URL usually contains the domain name, but if it contains an IP address, then there is a possibility of a phishing attack.
-	The “@” symbol: The case in which the “@” symbol is placed within the URL can make the browser go to a different address, which can be a phishing attempt.
-	“https” in Domain: Official or legal sites employ “https” for protected communication with the client.
-	URL shortening service: The actual link usually disguises itself, and phishers generally employ URL shortening services.
-	Prefix or suffix “-“ in the domain: Hyphens in the domain name can also be considered as a sign of phishing due to the tendency of phishers to use sub-domains to replicate definite websites.
 
Domain Based Features
The following domain-based features were considered: 
-	Website Traffic: It means traffic or popularity of the website when receiving traffic. A well-established website is generally more popular than a fake one.
-	End period of Domain: The period this domain has been registered. Cybercriminals registering the various phishing domains usually do so for shorter durations.


HTML based features
HTML-based features are the characteristics of the page that are extracted by analyzing the HTML code that describes the page's content.
-	IFrame Redirection: Similar to the case with referential metadata tags, the utilization of the IFrame tags to insert outside content can be exploited for unethical motives with the intention of concealing the genuine identity of a webpage.

