
British Airways Web Scraping and Analysis Projects
Overview
This repository contains three comprehensive projects analyzing British Airways' customer experience and operational data through web scraping, sentiment analysis, predictive modeling, and exploratory data analysis (EDA). The projects aim to uncover actionable insights to enhance service quality and operational efficiency for British Airways.

Projects
Web Scraping and Sentiment Analysis
Predictive Modeling for Customer Sentiment
Exploratory Data Analysis (EDA) of Flight and Rating Data
Article
https://medium.com/@abdulsalamibrahima017/unlocking-insights-a-deep-dive-into-british-airways-passenger-experience-f62e6cfff597
Presentation
https://docs.google.com/presentation/d/1Za0fjvwVDgwUDtpbk0lDIM5AiD2BVfoKlikpKDLK8Pk/edit?usp=sharing

Dataset Descriptions

B_Airways_ratings.csv
index: Index column
date_flown: Date of the flight
staff_service: Rating of the staff service (1-5)
food: Rating of the food service (1-5)
ground_service: Rating of the ground service (1-5)
seat_comfort: Rating of the seat comfort (1-5)
value_for_money: Rating of value for money (1-5)
recommended: Whether the reviewer recommended the airline (Yes/No)

B_Airways_flight_info.csv
index: Index column
date_flown: Date of the flight
travellers_type: Type of travelers (e.g., Business, Leisure)
route: Flight route
aircraft: Aircraft type
Seat_type: Type of seat (e.g., Economy, Business)

reviews.csv: Scraped reviews dataset.

Web Scraping
Overview
This project involves scraping customer reviews of British Airways from a third party website https://bit.ly/3VUEG0Z to understand the sentiment towards the airline. Sentiment analysis is to be applied to categorize the reviews into positive, neutral, and negative sentiments.
and for further exploration


Key Files
WebScraping.ipynb: Script for scraping reviews from websites.

Steps
Request all pages.
Locating tags.
Extrating tag text
Handling irregularities and alignment of data.
Structuring data into DataFrame.
Storing Datasets


Sentiment Analysis and prediction
Overview
This project focuses determining the sentiment of reviews and on building a predictive model to forecast customer sentiment based on review content. The model helps in identifying potential issues proactively.

Key Files
sentiment_analysis.ipynb: Script for performing sentiment analysis on the scraped reviews.
reviews.csv: Dataset of reviews with sentiment labels.

Steps
Loading the review data.
Tokenizing Lemmatizing review.
Detecting language using langdetect.
Extracting sentiments using TextBlob.
Preprocessing data by Creating Bag of Words (BOW)
Imputing missing data (most frequent strategy is used)
Build and train the predictive model.
Evaluate the model's performance.


Exploratory Data Analysis (EDA) of Flight and Rating Data
Overview
This project involves EDA of flight and rating data from 2019 to 2024 to identify operational patterns and customer preferences.

Key Files
eda.ipynb: Script for performing EDA on the flight and rating data.
B_Airways_flight_info.csv: Dataset containing flight information.
B_Airways_ratings.csv: Dataset containing flight ratings.

Steps
Load and clean the datasets.
Analyze and visualize patterns in flight data (e.g., most flown aircraft, popular routes).
Analyze and visualize customer ratings and service performance.
Identify areas for improvement and make recommendations.


Recommendations
General
1. Automated Data Cleaning: Implement automated scripts to clean and normalize the data, ensuring consistency and accuracy.
2. Incremental Scraping: Develop a system to incrementally scrape new reviews, keeping the dataset up-to-date without redundant data collection.
3. Enhance food and ground services to improve customer satisfaction.
4. Invest in more comfortable seating options for long-haul flights.
5. Explore new routes and increase frequencies to regions with growth potential.
6. Continue training programs for staff to maintain high service standards.
7. Enhanced Customer Service Training: The high volume of negative reviews indicates a need for improved customer service training, focusing on empathy, problem resolution, and communication skills.
8. Regular Monitoring and Feedback Loop: Implement a system for regular monitoring of review sentiments and a feedback loop where customer feedback is promptly addressed, and improvements are made.
9. Targeted Improvements: Identify common issues highlighted in negative reviews, such as delays, seating comfort, and service quality, and target these areas for immediate improvements.
10.Positive Reinforcement: Recognize and reward staff and service areas that receive positive reviews to encourage continued excellence.
11.Transparency and Communication: Increase transparency with customers regarding delays and service issues, and improve communication to manage expectations and reduce negative sentiments.
 



Conclusion
By leveraging insights from these projects, British Airways can proactively address customer concerns, enhance service offerings, and explore new growth opportunities. This repository provides the necessary scripts and datasets for replicating the analysis and driving data-driven decisions in the aviation industry.

How to Run
Clone this repository.
Install the required dependencies.
Run the scripts for each project as described in their respective sections.
bash
Copy code
git clone <repository_url>
cd <repository_name>
pip install -r requirements.txt
python <script_name.py>

License
This repository is licensed under the MIT License. See the LICENSE file for more details.

Contact
For any questions or suggestions, please contact Ibrahim Abdulsalam at Abdulsalamibrahima017@gmail.com or chat up +2349131606400