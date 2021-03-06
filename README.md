# Bert NLP text classification project
## Introduction
The purpose of this project is using numerous discussion text data from different forum websites and build a text classification model in order to predict what types of forums the discussions should belong to. 
## Data
All data files are stored in the folder "bert_data" in xlsx format. There are eight data files:
* folksy_forum_posts.xlsx  
Entries: 53776, Attributes: 13
* codecombat_forum_posts.xlsx  
Entries: 43504, Attributes: 13
* hopscotch_forum_posts.xlsx  
Entries: 53049, Attributes: 13
* schizophrenia_forum_posts.xlsx  
Entries: 13265, Attributes: 13
* bnz_forum_posts.xlsx  
Entries: 4191, Attributes: 13
* huel_forum_posts.xlsx  
Entries: 11956, Attributes: 13
* quickfile_forum_posts.xlsx  
Entries: 53460, Attributes: 13
* airline_forum_posts.xlsx  
Entries: 36398, Attributes: 13  
  
Attributes:
* post_text: str
* post_id: int
* user_id: int
* username: str
* reply_to_post_num: int
* topic_id: int
* post_num: int
* reply_count: int
* created_at: datetime
* updated_at: datetime
* num_reads: int
* topic_slug: str
* forum_name: str
## Method
* Web crawler  
talkfolksy-scraper/talkfolksy1/spiders/Main_page.py  
Web crawler for the discussion topics and contents on the main page of the forums.  
talkfolksy-scraper/talkfolksy1/spiders/Post_page.py  
Web crawler for the discussion contents on each topic page. 
* Bert NLP Text classification
model.py  

## Libraries  
* pandas
* numpy
* re
* torch
* transformers
* sklearn.linear_model
* sklearn.model_selection
* html2text
* DistilBertTokenizer
* torch.utils.data
* datetime

