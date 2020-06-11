# Drug-Reviews-NLP-Project
 The final project for the Natural Language Processing Course. Sentiment Analysis, Topic Modeling, collocation and entity extraction on the Drug reviews dataset - 'WebMD Drug Reviews Dataset'

### [The dataset](https://www.kaggle.com/rohanharode07/webmd-drug-reviews-dataset) in the center of this project provides user reviews on specific drugs along with related conditions they are used for, and ratings reflecting overall patient satisfaction. It also has columns for the medication's side effects that have occured to them if any, data about the patient's age, date it was reviewed and also two other types of rating: effectiveness and ease of use.
 ![Word Cloud of the reviews](https://scontent.fskp1-1.fna.fbcdn.net/v/t1.15752-9/103471440_937256416723689_6778015454068924338_n.png?_nc_cat=107&_nc_sid=b96e70&_nc_ohc=k5au7eE5kZ4AX85nkeJ&_nc_ht=scontent.fskp1-1.fna&oh=3673c408f265595046cda671afe394d5&oe=5F0753A1)

[The data](https://www.kaggle.com/rohanharode07/webmd-drug-reviews-dataset) was acquired by scraping [WebMD site](https://www.webmd.com/). There are 362 769 unique reviews and contains data from 2007 till March 2020.
https://www.kaggle.com/rohanharode07/webmd-drug-reviews-dataset

- In the first Jupyter notebook ***"1_Visualization_of_the_dataset_and_some_exploratory_data_analysis.ipynb"*** we get to have a deeper look at the data with some exploratory data analysis techniques.
- The second notebook ***"2_Topic_Modeling_with_LDA,_Collocations_and_entity_extraction_using_SpaCy.ipynb"***
contains the approach of Topic Modeling with LDA, but it has not given the expected satisfying results.
Next step is aplication of collocation for discovering meaningful phrases that come up often in the 
reviews about the medications. This kind of information may be used  for labeling important information 
about the comments for the drugs. Generating this kind of meaningful phrases (if they are marked down,
for example in bold text) help us as people, even if we are
just reading them, to extract information easier and within a less amount of time, notice what is the important
part of a review that deserves our attention.
Next up, was training a (SpaCy) model for recognising a new custom entity 'DRUG' in the reviews which is pretty simple, but it can have interesting applications.
This type of functionality can be useful if for example, the patient in her/his review has 
stated experience with some contraindications or improvement thanks to a combination with another 
entity marked as 'DRUG'. This type of feature can be used for some kind of drugs recommendation system creation.

- The third notebook - ***"3_Sentiment_analysis_with_VADER,_Multinomial_Naive_Bayes,_Decision_Tree,_Random_Forest_Classifier,_KNN,_Gradient_Boosting,_XGBoost_and_SVM.ipynb"*** attempts to give answers 
about identifying the meaning of the patient's opinion about the medication using different 
algorithms and models and finally comparing the results they give under these conditions - for this specific data processed with those specific preprocessing 
techniques. Sentiment analysis lets us understand the subtle differences in the reviews and locate 
where does the problem or positive experience originate from.
