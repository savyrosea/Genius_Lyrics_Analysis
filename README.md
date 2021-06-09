# Genius_Lyrics_Analysis

View the Final Lyrics Analysis Here: https://sites.google.com/view/geniuslyricscapstone

### 0. Data Questions
- What do aspects such as amount of profanity and common phrases tell us about today's music?
- What emotions/ sentiments are most commonly communicated in today's popular music?
- Can we create a model that will generate new lyrics given a corpus of lyrics?

### 1. Gathering the Data
- For this project I defined a popular artist as an artist who has appeared on Billboard Top 100's list during 2019, 2020, or 2021 (Jan-April). After gethering a list of artists from Billboard, I used Genius API to collect data such as artist description as well as the lyrics for each artists top 15 songs. This gave me a "Artist" data set with 115 unique artists and a songs data set with 1725 songs.

### 2. Data Cleaning

- Artist gender was scraped from the artist's description text. If the text referred to the artists with he/him the artist was marked as male and if the artist was referred to as she/her the artist was marked as female. A list of non-binary artists was used to overwrite the few non-binary artists with their correct gender. The remaining artists were assumed to be a group and have a Null value for gender.

<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/genderbar.png" width="350" />
</p>

- Artist Birth Date was scraped as the first 4 digit number following the artists name. In the artist description the birth year is in a consistant format following the artist name.
- 
<p float="left">
  <img src="https://github.com/savyrosea/Genius_Lyrics_Analysis/blob/main/pictures/agehist.png" width="290" />
</p>

- From here I started preprocessing the text data for further use in n-grams and sentiment analysis. I remove stopwords (except for in lyric generating models) and removed cues in lyrics indicating who was singing or the part of the song.

Examples: [Verse 1:], [Chorus], (Post Malone), (Ariana Grande)

I also cut down on repetition in songs as it would skew my n-gram results and I removed numbers and other unusual characters.

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
