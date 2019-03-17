# social_media_misc
Learning from others

# Sentiment Analysis
----------------------
Analyze the Twitter posts sentiment by texts and tags

I really like the work of the Stanford NLP lab
http://nlp.stanford.edu:8080/sentiment/rntnDemo.html, which can generate almost 100% correct sentiment of my typings (yeah, some very simple typings)

I am proposing this project to see there is a better way to do Sentiment Analysis. 

According to [Mullen](/ref/mullen.pdf): 
* **Sentiment Analysis(SA)** is Using NLP, statistics, or machine learning methods to extract, identify, or otherwise
characterize the sentiment content of a text unit 
* It has comparatively few categories (positive/negative, 3 stars, etc) compared to text categorization
* The SA is **challenging** because 
 * People express opinions in complex ways
 * In opinion texts, lexical content alone can be misleading
 * Intra-textual and sub-sentential reversals, negation, topic change common
 * Rhetorical devices/modes such as sarcasm, irony, implication, etc. 
* We need to decide **what** we want to classify, a.k.a, our analysis unit
 * Users/Texts/Sentences/Short Phrases/Words/Tweets(short text updates)
* **Methodology**
 * Polarity Keywords: Correlation between positive words and positive reviews
 * Smileys: The emoticon/emoji/smiley says a lot about your tweet
* **Existing Tools**
 * LIWC (Linguistic Inquiry and Word Count) 
 * Wordnet (A lexical database for English with emphasis on synonymy) --> SentiWordNet: Each synset is assigned three sentiment
scores: positivity, negativity, and objectivity
* **Existing Datasets**
 * [Pang & Lee data sets](http://www.cs.cornell.edu/People/pabo/movie-review-data/): moving ratings and reviews
 * [Blitzer et al Multi-domain sentiment dataset](http://www.cs.jhu.edu/~mdredze/datasets/sentiment/): Amazon rating and reviews
 * I can find more on Kaggle or crawl myself 
* **Techniques**
 * Semantic orientation and polarity of words (no gradient,Manually classed, single word only, Blind to context) 
 * Evaluate the popularity of sentence (pre-defined noun, count of negative and positive words)
 * Osgood values for words using WordNet (Yields a list of adjectives with EVA, POT and ACT scores) 
 * Semantic orientation of phrases
 * Text-based sentiment classification: The PMI-IR method yields real-numbered positive and negative scores for potentially any combination of words
 * Incorporating shallow linguistics
 * SVM to combine information from multiple resources
 * Topic information is very important 
 * word and phrase based features
 * Other approaches
* **To Sum Up** 
 * The difficulty of SA increases with the nuance and complexity of opinions expressed
 * Product reviews, etc are relatively easy
 * Books, movies, art, music are more difficult
 * Policy discussions, indirect expressions of opinion more difficult
 * Non-binary sentiment (political leanings etc) is extremely difficult





#### Ref
* https://rstudio-pubs-static.s3.amazonaws.com/124656_e2e77362772d40a4a7be244d2f114853.html#/
* https://lct-master.org/files/MullenSentimentCourseSlides.pdf
* Coursera NLP by Stanford

