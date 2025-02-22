# AI-Powered Personalized News Aggregator

## Objective
The goal of this project is to build an AI-powered Personalized News Aggregator that scrapes, filters, summarizes, and recommends news articles based on user preferences. Using Natural Language Processing (NLP) and Machine Learning (ML) techniques, this system enhances user experience by providing concise, relevant, and personalized news summaries.

## Key Tasks Performed

**News Scraping & Data Collection**
   
•	**API Used:** NewsAPI.org

•	**Categories Covered:** Technology, Sports, Business

•	**Process:**

    o	Fetches top headlines for each category.
    
    o	Extracts key information like title, description, and content.
    
    o	Saves the news data into a structured CSV file for further processing.
    

**Filling Full Content for Each Article** 

•	**Challenge:** Some news sources provide incomplete or truncated content.

•	**Solution:**

      o	Implemented web scraping (using BeautifulSoup) to fetch full content for articles missing details.

      o	Integrated fallback mechanisms to ensure complete and accurate data before summarization.

**News Summarization**

•	**Model Used:** facebook/bart-large-cnn (BERT-based text summarization)

•	**Process:**

      o	Extracts relevant parts of the article content.
      
      o	Generates a concise summary while retaining key information.
      
      o	Handles missing or incomplete data gracefully.
      

**Sentiment Analysis**

•	**Tool Used:** VADER (Valence Aware Dictionary and sEntiment Reasoner)

•	**Process:**

      o	Analyzes news content to determine Positive, Neutral, or Negative sentiment.
      
      o	Assigns a sentiment score and labels articles accordingly.

**News Recommendation System**

•	**Model Used:** Sentence Transformers (all-MiniLM-L6-v2 for BERT embeddings)

•	**Process:**

      o	Converts article summaries into vector embeddings.
      
      o	Computes semantic similarity using cosine similarity.
      
      o	Recommends similar articles based on user interests.
      

## Outcome & Conclusion
### Outcome
**Successfully built a Personalized News Aggregator that:**

      o	Scrapes, summarizes, and categorizes news articles.
      
      o	Conducts sentiment analysis to help users gauge article tone.
      
      o	Uses AI-driven recommendations to suggest relevant articles based on user preferences.
      
      o	Provides a scalable and customizable framework for real-time news processing.


### Conclusion

This project demonstrates the power of NLP and Machine Learning in delivering a tailored and enhanced news-reading experience. The combination of BERT-based summarization, sentiment analysis, and AI-driven recommendations makes the aggregator highly efficient and user-friendly. Future enhancements may include:

      •	User authentication to store personalized preferences.
      •	Topic modeling for better article categorization.
      •	Real-time notifications for breaking news updates.

 Next Steps:
      •	Deploy the system using Streamlit for a user-friendly UI.
      •	Explore more advanced deep learning models for text analysis.
      •	Expand the news sources beyond NewsAPI for diverse coverage.

