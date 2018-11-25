# Investing for Social Good

# Abstract
*"Society is demanding that companies, both public and private, serve a social purpose. To prosper over time, every company must not only deliver financial performance but also show how it makes a positive contribution to society."* - Laurence D. Fink, CEO BlackRock (largest asset manager in the world)

Asset managers are increasingly challenged by their investors to manage their portfolios for social impact. However, it is non-trivial for investors and investment managers to maintain regular oversight over the social impact composition of their portfolios. The U.S. Securities and Exchange Commission’s (SEC’s) EDGAR maintains a digital record of the portfolio filings of publicly traded asset managers. All the News is a Kaggle dataset of news articles primarily from 2016 to 2017. 

Furthermore, it could be interesting to correlate the greater public's interest into social good projects expressed on social media platforms such as Twitter and Facebook, or news platforms, with the actual investments that are done. 

# Research questions
- How to map news article sentiments to specific investments held by companies?
- What are the most popular “ethical” or “unethical” investments held by asset managers?
- What asset managers have the portfolios with the greatest/least social impact?
- What is the great public's opinion regarding the companies that held many investments in social good versus those who do not invest in social good? 
  - How to make a ranking of “public opinion” regarding a company? 
- Was there a transition toward investing more into social good then into other projects? If yes, when did it happen? 
- Can we extend the project to other countries in other to build a global social good investment chart? 

# Dataset
List the datasets containing the information needed to answer the above-mentioned questions: 

- [The news][https://www.kaggle.com/snapcrack/all-the-news/home] (253 MB)

- [SEC asset manager portfolios][https://www.sec.gov/cgi-bin/browse-edgar?company=&CIK=&type=13F&owner=include&count=40&action=getcurrent]
- Twitter : 1% of the tweets of 2017 

Once the project topic was chosen, the group spent a considerable amount of time to look at the quality of the data. For the members, it was important to make sure that the time allocated to the project will be spent on data science and information extraction and not data cleaning.

Our group found some libraries to generate a .csv-like file listing, by company and date, the URLs in the SEC's archives where the investment portfolio filings are stored (https://github.com/edouardswiac/python-edgar) as consistently structured text and HTML table data. We will be able to programmatically extract the type and scope of different types of asset manager investment holdings (what companies they invested in, the size and value of each investment). This data can be enriched by processing additional news and social data related to portfolio companies into signals of their social impact and mapping these social impact signals to investment portfolios. Based on this data from investment portfolio filings, we hope to be able to identify and analyze investments made in companies that pursue goals related to *social good* from all different kinds of industries. 

Regarding the dataset on kaggle, we took a closer look to the comments made about the data and we found no issues. Moreover, the download of the 3 .csv files was done. The structure is well defined with several columns (title, publication, author, data, year, month, URL, content). The size of the dataset is small. 

The Twitter data is a dataset provided by the course so we are confident that there should not be too many insolvable issues and the data does not look *too bad*. The documentation of Twitter API was analyzed to understand how to use this database. First, determination of a dictionary of keywords linked to our subject will be done (and possibly Machine Learning algorithms will be used to broaden it throughout work process). Finally, the tweets will be filtered thanks to the buolt dictionary in order to construct the dataset of interest.

# A list of internal milestones up until project milestone 2
- Milestone 1 (M1) 
  - Task Group 0
    - [x] Download the required data
    - [x] Set up the Git and Project plan
  - Prepare Milestone 2 
    - [x] Comment and debug the code : *Through the homeworks, we learnt how to work together as a team of 3 students. Throughout this learning process we also learnt which comments in the code are useful for the other members of the team and which comments were not that usefull. Obviously, this process is not over but we got way better than in week 1.*
    - [x] Learn from the mistakes made in M1
    - [x] Set clear goals and plans for the next milestone : *The ... *
  - Task Group 1 - Data Exploration
    - [x] Clean and organize our data
    - [x] NaN values, how can we deal with bots and spam etc. (Read papers that might give us interesting insights)
    - [x] Establish a process for performing tests and evaluations on smaller parts of the dataset and understanding to what extent we will need to work within the frameworks of the cluster
    - [x] Understand how the cluster works
  - Task Group 2 - Data Exploitation
    - [x] Explore data visualization possibilities
    - [ ] Decide which visualizations formats serve the best our purpose.
    - [x] Exploration of pre-trained simple Natural Language Processing (NLP) methods (LSI, pLSI, LDA and VSM using lemmatization, stemming and n-grams) to perform analysis on the Twitter and news datasets.
    - [ ] Determine a dictionary of keywords linked to emotion and opinion identifiers regarding companies. 
    - [ ] Process and perform a detailed analysis of the news and SEC asset manager datasets, perform data wrangling and preprocessing.
  - Task Group 3 - Wrapping up MS1  
    - [ ] Process and perform a detailed analysis of the news and SEC datasets, filtering out the relevant data and understand how to combine the two datasets with the information on Twitter for instance.
    - [ ] Find trends in the data regarding the social opinion to the investors and correlate it with the findings regarding the investments done by companies. 
  
#### Questions for TA's

- What technologies do professional data blogs like FiveThirtyEight use for visualization?
**ANSWER** : *For fancy visualisation, you can use D3.js, for simple one you can use some wrappers of D3.js (C3.js)* 
- Is the content we have enough to make a project?
**ANSWER** :  *You seem to have enough content for now. Once you start exploring the dataset you can reiterate on your research questions and refine them if needed.*
