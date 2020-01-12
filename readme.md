###Final project

Team members: Ron Mizrahi, Samuel Guerchonovitch, Yona Eisenberg

Project title: Fake news and stance detector in political articles

Datasets: politifact.com 'truth-o-meter' defining how likely a political/news statement is of being true or false - about 17K of labeled data on american politics

Description
Given an article (headline, source, date, content, and so on...), predict whether it is fact or fake.

As a enrichment, we could have a stance detector, given an two sentences from one or several articles, classifying it as 'agrees', 'disagrees', 'discusses','unrelated', and use this detector and data enrichment from reliable medias sources to improve our detector performances. Eventually, it would allow us to create a metrics of correlation between different articles, and use the base dataset to predict truth likelihood for outside articles.

Measure of success: 
At first accuracy/precision/recall between our model and the labeled data from the original website (splitting to train and test)
Then taking outside articles that we know are facts/fake and measuring accuracy/precision/recall on them.


Right direction 3-weeks objective:
- Successfully webscrape the base dataset from politifact.com
- Basic classifier for our base dataset (even with bad performances)


Risk of failure:
- Bad bias on the base label (if the website is biased or uses a low threshold for fact checking)
- 'Unrelated' relation between a lot of articles and the sentences because of missing data in the base dataset

