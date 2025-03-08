## Political Polarization through Reddit: Analysis of Democrat and Republican Communities

### Team 4, LSE Data Science Society

### Project Overview:

This project explores political polarization through Reddit, specifically in the subreddits 'democrats' and 'republicans'. The goal is to understand how political polarization manifests in language, sentiment, and media preferences.

* **Data Sources:**
   * Reddit 'democrats' and 'republicans' subreddits.
   * Data collected using the PRAW API.
   * 1000 posts from each subreddit, focusing on "hot" posts from the time window of December 2023 to December 2024.

### Key Insights:
1. **News Source Polarization:**
   * Democrats prefer progressive sources like *Newsweek*, *Raw Story*, and *HuffPost*.
   * Republicans favor conservative outlets such as *Fox News*, *Breitbart*, and *Not The Bee*.

2. **Sentiment Analysis:**
   * Sentiment divergence was observed between subreddits using VADER sentiment scoring.
   * Mood shifts were tracked over time to understand emotional trends around political events.

3. **Linguistic Differences:**
   * Word clouds visualized differences in language, with Republicans focusing on campaign and strategy terms, while Democrats discussed legal issues and policy criticisms.

4. **Classifier for Polarization:**
   * Logistic Regression and deep learning (Bidirectional LSTM) models were used to classify posts by subreddit, achieving decent performance.

### Technical Details:
* **Data Features:**
   * Title, score, ID, URL, number of comments, created timestamp, body content.

* **Sentiment Analysis:**
   * Used VADER for sentiment scoring and analyzed sentiment across posts.

* **Word Cloud Generation:**
   * Combined all post titles and created a word cloud to highlight frequently used terms.

* **Machine Learning:**
   * TF-IDF features were used for logistic regression and LSTM classifier.


### Results:
* **Classifier Performance:**
   * The LSTM model showed improved recall for Democrat posts (0.74), although accuracy was marginally improved over Logistic Regression.

* **Insights:**
   * Political discourse on Reddit is highly polarized, with distinct ideological differences observed in language, sentiment, and media preferences.

### Conclusion:
* **News Source Polarization:**
   * The analysis confirms that news sources on both subreddits are highly polarized, reinforcing ideological divides.
   
* **Sentiment Divergence:**
   * Sentiment scores reflect distinct emotional responses to political events.

* **Word Cloud Analysis:**
   * The linguistic analysis revealed distinct focuses and themes between Democrats and Republicans.

* **Classifier:**
   * While the classifier performed reasonably well, further improvement is needed for real-world applications.

### References:
1. Pew Research Center, *U.S. Media Polarization and the 2020 Election: A Nation Divided*, [Link](https://www.pewresearch.org/journalism/2020/01/24/u-s-media-polarization-and-the-2020-election-a-nation-divided)
2. Ross Arguedas, A., Robertson, C., Fletcher, R., & Nielsen, R. (2022). *Echo chambers, filter bubbles, and polarisation: A literature review.*
