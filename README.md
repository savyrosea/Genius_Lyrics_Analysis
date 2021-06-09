# Genius_Lyrics_Analysis

View the Final Lyrics Analysis Here: https://sites.google.com/view/geniuslyricscapstone

### 0. Data Questions
- What do aspects such as amount of profanity and common phrases tell us about today's music?
- What emotions/ sentiments are most commonly communicated in today's popular music?
- Can we create a model that will generate new lyrics given a corpus of lyrics?

### 1. Gathering the Data
- Billboard Top 100
- Genius API
- Number of Artists and Songs

### 2. Data Cleaning

- Gender

<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/genderbar.png" width="350" />
</p>

- Artist Birth Date
- 
<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/agehist.png" width="290" />
</p>
- Text Preprocessing

### 3. N-Grams
- Top 2 Word Phrases by Gender and Age
- Top Word By Decade

### 4. Profanity Analysis
- Profanity By Artist

- Profanity By Gender
<p float="left">
  <img src="hhttps://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/prof.png" width="350" />
</p>

- Profanity By Age
<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/profLine.png" width="450" />
</p>

### 5. Sentiment Analysis
- VADER (Positive Vs. Negative)
- 
- NRC Lexicon

<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/sad1.png" width="250" />
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/surprise3.png" width="250" />
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/anger2.png" width="250" />
</p>

### 6. Generate a Pop Song
- Probability Model
- PEGASUS Summarization Model
-
























## Game Plan:
### Saturday, May 22nd:
  - Data Cleaning: Dates to Datetime :heavy_check_mark:
  - Data Cleaning: Get Artist Gender from Text :heavy_check_mark:
  - Data Cleaning: Get Artist Age from Text :heavy_check_mark:
  - Data Cleaning: Get Rid of Songs Not in English :heavy_check_mark:
  - Data Cleaning: Bring in Song Genre ❌
  - Pre-Process Text for N-Grams :heavy_check_mark:
 
### Sunday, May 23rd:
  - Pre-Process Text for N-grams (get rid of repitition in songs?) :heavy_check_mark:
  - N-Gram Analysis by gender :heavy_check_mark: 
  - N-Gram Analysis by age :heavy_check_mark: 
  - N-Gram Analysis by genre ❌
  
### Tuesday, May 25th:
  - Profanity-Check Library :heavy_check_mark:
  - Create Binary Column for if Song has Profanity or Not :heavy_check_mark:
  - Get Profain Probability % by Song :heavy_check_mark:
  - Get Profain Probability % by Artist :heavy_check_mark:
  - Get Profain Probability % by Artist Gender :heavy_check_mark:
  - Get Profain Probability % by Artist Age :heavy_check_mark:
  - Look for Correlations :heavy_check_mark:
  
### Thursday, May 26th:
  - Sentiment Analysis by Artist (NRC lexicon) :heavy_check_mark:
  - Create Function to get Numeric Values for Emotions Attached to Each Song :heavy_check_mark:
  - Sentiment Analysis by Song :heavy_check_mark:
  - Sentiment Analysis by Artist :heavy_check_mark:
  - Sentiment Analysis by Artist Gender :heavy_check_mark:
  - Sentiment Analysis by Artist Age :heavy_check_mark:

### Saturday, May 29th:
  - Use NLP to "Create" a pop song (probabilistic Bigram or Trigram Model or GPT-2 Model) ❌
  - Create pop song lyrics using statistics (probabilty of words that follow each other) :heavy_check_mark:
 
### Sunday, May 30th:
  - Gensim Topic or LDA Analysis (If time) ❌
  
### Tuesday, June 1st:
  - Artist Sentiment Negative to Positive on a -1 to 1 Scale
  - Hugging Face to Enhance Lyric Generation 
  - Set up Google Sites
  - Bring in Artist Photos or Album Artwork
  
### Thursday, June 3rd:
  - Wrap up Google Site 
  - Make Presentation
  
### Saturday, June 5th: 
  - Internal Demos
  
### Sunday, June 6th: 
  - Make Final Adjustments
  
### Tuesday, June 8th: 
  - Make Final Adjustments
  
### Thursday, June 10th: 
  - Demo Day
