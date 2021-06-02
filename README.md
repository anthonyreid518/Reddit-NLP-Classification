## Problem statement

This is a natural language processing project that takes two similar subreddit’s comments and applies various machine learning algorithms to identify the difference between them. The goal is to build a model that can differentiate between “machine learning” and “artificial intelligence” subreddit comments. Classification models such as decision tree, logistic regression, and naive Bayes have been considered	for this project and will be scored based on accuracy. There are 5,000 subreddits comments for each section, so success will be considered	as anything higher than 50% (ie only guessing one subreddit).  This is important to investigate in order to understand how we can train models and improve on them by providing more data. 

Which machine learning algorithm can accurately predict the difference between machine learning and artificial intelligence subreddit comments. 

## Executive summary

Natural Language processing (NLP)  is one of the many use parts of machine learning. This project uses NLP classification algorithms to determine the difference between Machine Learning and Artificial Intelligence subreddits. Comments from reddit were used as text data through a web scrapping method. The comments were placed into a dataframe and saved as a csv file shown in this repository. Below shows a table of the subreddit and the number of terms missing. We had 5,000 from each so the missing terms did not affect our model 

| Subreddit | Missing Terms |
| --- | --- |
| **ML 'removed'** | 20 |
| **ML 'deleted'** | 62 |
| **Ai 'removed'** | 36 |
| **Ai 'deleted'** | 75 |

Several classification models were tested and scored based on their accuracy	and balanced accuracy. The top performing models were Logistic Regression, Random Forest, and Naive Bayes which were all used in the final model as part of an ensemble. The models had a 78% accuracy score on the final test set. Although the model performs well on reddit comments, it can’t predict messages out of context well and is subject to hacking by typing ‘ai’ or ‘ml’. 

More work can be done to improve the model in the future such as incorporating titles from Reddits and using other sources for text such as news or articles. 


## Directory 

| File | Explination |
| --- | --- |
| ml_csv | Dataframe of the comments scrapped from the ML subreddit.  The first column is the subreddit label, the second column is the commnet made on the website. |
| ai_csv | Dataframe of the commetns scrapped from the Ai subreddit. The first column is the subreddit label, the second column is the commnet made on the website. |
| project 3.ipynb | Jupyter lab notebook that contains scrapping, cleaning, and analysis performed on this project.  |
| project3_Anthonypdf | Powerpoint slides in pdf format showing the process of this project and the key findings |

## Conclusion

Text from ML and Ai subreddits were scrapped, cleaned, and passed through several classification models for evaluation and comparison. Several models had the same performance on the test set and were later selected to be part of an ensemble. The NLP model is good at predicting these comments but can’t be used out of context. More training data is always helpful, include titles or text from different sites and articles. 