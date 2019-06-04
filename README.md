# Web-crawler-for-US-salary-predictions
This web crawler crawls through Indeed.com to scrape job title, location, salary for Tech professionals all over the USA and helps to make predictions through linear, logistic regression, KNN , neural networks, Random forest models to arrive at the best states and titles against the Median salary predictions in each role and state. The details of the workings of the crawler are explained within the jpynb and also i have created attractive visualizations in tableau dashboard for the same and uploaded the file here for reference.

Overview
The goal of this project is to help automate the recruiting process. To do this, we would like for you to create a service that crawls through indeed searching for qualified candidate leads .

This will touch every major process within the data pipeline:

Data Collection
Data Processing
Data Anayltics
Display / Use
1) Data Collection
Like the rest of this project, this will be done in Python. The goal is to create a web crawler / scrapper that searches through linkedin for software engineers at major companies. The choice of crawler is up to you, I have personally used Selenium before for Python, however it may be to robust for your purposes. You can use this guide as good starting point when 

Emulate that human behavior with a web crawler
2) Data Processing
Once a software engineer is found, their linkedin page should be parsed from HTML. This can be done using python's BeauifulSoup module. From there you can format it for anaysis.

Given a url to an indeed page, obtain the html data for that page (use the requests module within Python)
Process html using BeauifulSoup
Clean data however you need for the data anayltics
3) Data Anayltics
This is where most of your design and data creativity can come from. The hope is to create a statistical ranking of a given indeed page. This would be in the form of a percentage of how confident your algorithm is that the given indeed candidate is a good job and salary. 

Translate those metrics into a model that ranks a page (mostly nlp combined with anything else you deem nessary to the model)
Implement that model within python with any modules you need. (I'd recommend leveraging the NLTK module)
4) Display / Use
We will be utilizing this as an independent service; a service being an API that can be called by our main web service. This API can be created using either Pythons Flask or Django depending on preference (I personally have experience with Flask however Django is more utilized in industry). It will then be deployed to the cloud using AWS Elastic Beanstalk or Heroku (Tresten will decide based on future design descisions).

Wrap your code in a web service (API's) using Flask or Django
Create an API that accepts a linkedin URL and returns the confidence score
Create an API that can be called and will return a list of the top linkedin URL's found by the web crawler
Deploy this API for use on the cloud
Summary and suggestions
This project fits a direct business need to find job rankings as per location and salary.
