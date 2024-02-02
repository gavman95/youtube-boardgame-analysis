# Exploratory Data Analysis (EDA) of 4 Board Game Youtube Channels

## Table of Contents

1. [Introduction](#introduction)

   1.1 [Aims, Objectives, and Background](#aims-objectives-and-background)

2. [EDA & Insights](#eda-and-insights)
   2.1 [Video Metrics](#video-metrics)
   
   2.2 [Subscriber Count](#subscriber-count)
   
   2.3 [Top 10 Viewed Videos](#top-10-viewed-videos)
   
   2.4 [Upload Schedule](#upload-schedule)
   
   2.5 [Relationship of Likes/Comments vs View](#relationship-of-likes-comments-vs-view)
   
   2.6 [Sentiment Analysis](#sentiment-analysis)
       2.6.1 [Popular Themes](#popular-themes)
       
       2.6.2 [Top 10 Videos Based on Their Sentiment Scores](#top-10-videos-based-on-their-sentiment-scores)
       
       2.6.3 [Inquiries in Comments](#inquiries-in-comments)
       
       2.6.4 [Decrypto Board Game](#decrypto-board-game)
       
       2.6.5 [Choosing 2 Channels to Follow](#choosing-2-channels-to-follow)

3. [Conclusion](#conclusion)

## Introduction <a name="introduction"></a>

Playing board games is one of my favorite hobbies when spending time with friends and family. I love the problem-solving, creative thinking, teamwork, and competitive nature involved in playing board games. Especially when trying out a new game for the first time, the anticipation and understanding of how the game is designed are intriguing. I wanted to search for a YouTube channel centered around board games in the hopes of watching friendly competitive games and discovering any new board games that might interest me.

Four channels I came across, which I was interested in, are Acualol, The Dice Tower, Good Time Society & No Rolls Barred.

### Aims, Objectives, and Background <a name="aims-objectives-and-background"></a>

Within this project, I would like to explore the following:

* Exploring how the YouTube API works and how to retrieve video data.
* Analyzing the data of the videos and exploring some questions, for example:
  * Does the number of likes and comments matter for a video to get more views?
  * Top 10 videos based on views.
  * Subscriber count.
  * What has been the upload schedule throughout each channel's history?
* Explore NLP techniques using sentiment analysis.
  * Which popular themes are uncovered in the videos.
  * Based on the comments section, what is the sentiment of the videos?
  * What inquiries are being posed in the comment sections of the videos?
  * How have the videos exploring the game Decrypto been received by viewers based on the comments?

## EDA & Insights <a name="eda-and-insights"></a>

### Video Metrics <a name="video-metrics"></a>

| channel_name       | description                                           | total_views | total_uploads | total_subscribers | channel_unique_playlist_id |
|--------------------|-------------------------------------------------------|-------------|---------------|-------------------|-----------------------------|
| Good Time Society   | Welcome to Good Time Society! Stick around awh...    | 4559173     | 553           | 58100             | UUBRTbbK-avyRJSSJ2GyHs_w    |
| The Dice Tower      | Video reviews of games, top 10 lists, live pla...    | 332478165   | 23180         | 334000            | UUiwBbXQlljGjKtKhcdMliRA   |
| No Rolls Barred     | Welcome to the Official No Rolls Barred YouTub...    | 57216291    | 365           | 320000            | UU5UQPZe-8v4_UP1uxi4Mv6A   |
| Actualol            | Board game reviews with a sense of humour.           | 8584495     | 189           | 106000            | UUO-hn9MJOu7pOUdGSabKGvA   |


### Subscriber Count <a name="subscriber-count"></a>

Just to get things started off, I wanted to create a plot of the channels and their subscribers count. As we can see, The Dice Tower is the most followed channel at 334K, followed by No Rolls Barred at 320K, then Actualol at 106K, with Good Time Society being the least followed out of the four channels at 58.1K.

![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/ebbe76d6-d624-4da7-aaae-d38562fa98e9)

### Top 10 viewed videos <a name="top-10-viewed"></a>
Next I wanted to visualise the top 10 viewed videos and top 10 liked videos. It was found that 6 out of the top 10 viewed videos were from the No Rolls Barred channel, with 3 belonging to The Dice Tower and 1 to Actualol. In regards to the top 10 liked videos, 8 videos belonged to No Rolls Barred Channel and 2 to Actualol.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/b7c64482-c613-4d9a-9e01-dd20f43ab781)
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/afbf03f5-846b-4f93-89a0-37579b5cb284)


### Upload Schedule <a name="upload-schedule"></a>

From the below visualisation, its interesting to see the different variety in the upload schedule of diiferent channels. For example Actualol mostly uploads their videos on weekdays, especially on Wednesday being the peak and closely followed by Thursday. Barely any videos are uploaded on the weekend, with just a few on Sunday. For The Dice Tower its a bit different with there quite being of an even spread in which days videos are uploaded, for example Tuesday, Wednesday, Thursday, Friday & Saturday all have similar number of uploads in the channels history. This could be as a result of change of upload schedule over time with The Dice Tower first upload in the year 2014. On the other hand, No Rolls Barred is the most recent channel to be set up (in 2020) compared to the other 4, and its upload schedule is distinct, with the majority of uploads occuring on Tuesday & Saturday. Finally, for Good Time Society, most uploads occured on Tuesday and then history of uploads drop each day.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/f5611c61-b23f-47d3-bd96-2efb6da4e072)

### Relationship between number of likes or comments vs number of views views? <a name="relationship-of-likes-comments-vs-view"></a>

From the below observation, the next thing I wanted to explore was whether number of likes or comments correlate with how many views a video reaches. From the scatterplots below, it can be seen that the number of views is strongly correlated with the number of comments/ likes of the video. The more number of likes or comments in a video, likely the more views. This is expected as with a larger audience size, there is the tendency for more engagement in a video.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/0344821e-8527-490f-aefc-01e3d698f301)

### Sentiment Analysis <a name="sentiment-analysis"></a>

#### Popular Themes <a name="popular-themes"></a>

Now I wanted to get a feel of the polarity for what the channels where about. Obviously I know these channels are about board games but it would be good to visualise the more frequently used word in the title of the videos. As we can see the terms like "Board", "Game", "Review", "Unboxing", "Dice", "Play" are common themes with board game lore and show up in lots of the videos titles

![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/bb74e86e-7cf3-4e52-b501-2fea4c445353)

#### Top 10 videos based on their sentiment scores <a name="top-10-sent"></a>
From the plots below, it was interesting to find that whilst the top 10 viewed videos mostly had a positve sentiment, the sentiment score wasnt as high as those compared to the top 10 videos based of sentiment score. This could be the more views a video accumualtes, the more comments it gets leading to a larger diverse comments environment.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/4b85e4e5-8437-483a-807c-ac8d00eca380)

When comparing the top 10 viewed videos vs top 10 videos based on sentiment, it was clear there was a large difference in the mean view count, from 1147724 vs 10770.

```python
loo = pd.DataFrame(top10[['title','viewCount','sentiment_score','publishedAt','duration']])
loo=loo.reset_index(drop=True)
print(f'mean view count: {loo.viewCount.mean():.0f}')
print(f'mean sentiment score: {loo.sentiment_score.mean():.2f}')
print(f'mean duration: {loo.duration.mean():.0f}')

 Output:
 mean view count: 1147724
 mean sentiment score: 0.14
 mean duration: 3068

lool = pd.DataFrame(top10_sent[['title','viewCount','sentiment_score','publishedAt','duration']])
lool=lool.reset_index(drop=True)
print(f'mean view count: {lool.viewCount.mean():.0f}')
print(f'mean sentiment score: {lool.sentiment_score.mean():.2f}')
print(f'mean duration: {lool.duration.mean():.0f}')

 Output:
 mean view count: 10770
 mean sentiment score: 1.00
 mean duration: 1094
```

#### Inquiries in Comments <a name="inquiries-in-comments"></a>

Videos with a mean sentiment score over 0.05 where deemed to have a positive sentiment. The wordcloud below identfies common words within the positive sentiment videos such as "game", "great", "love", "thank", "favorite", "good",e.t.c all thematic words indicating of a consensus of a positive video

![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/bbffd86c-4c7d-424b-8ff8-aacf29406c71)

#### Decrypto??? What is the vibe on this game <a name="decrypto"></a>

One of the games which I have heard for a long time but havent played is Decrypto. From the 4 channels I wanted to see if they made videos on this game and get a feel of the sentiment. I was happy to see out of all the videos for Decrypto, not one had a mean negative sentiment score, with 6 out of the 8 videos all scoring a positive sentiment whilst the other 2 were neutral. Maybe once I too watch these videos I might purchase the game.

Again I made a word cloud for videos related to Decrypto and mostly positive words were frequently shown in the comments as expected.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/1c25547b-4bec-4293-9158-165c51e48584)

#### Chosing 2 channels to follow <a name="choosing-two-channels"></a>
Initially, what puts me off about the Dice Tower channel is that although it has the highest subscriber count and the highest number of uploads, its mean view count is the second lowest, and it has the lowest positive sentiment score out of the 4.

Despite having a substantial subscriber count and a significant number of uploads, the lower mean view count and sentiment score could suggest a few possibilities:

1. **Diverse Content:** The channel may have a wide variety of content, and some videos may resonate more with the audience than others. This diversity can impact the average view count and sentiment.

2. **Audience Expectations:** Subscriber count doesn't guarantee that every subscriber watches every video. The expectations of the audience may vary, affecting the level of engagement. It could be that subscribers aren't as engaged as they once were with the channel.

#### My Preferences

**Hypothetical Preferences:**

- Preference for a positive and engaging atmosphere.
- Moderate to high average view counts are important.
- Enjoy a mix of content lengths, including both shorter and longer videos.

**Analysis:**

1. **Actualol:**
   - High mean sentiment score (0.45), indicating a positive atmosphere.
   - Moderate mean view count (45,452).
   - Shorter mean duration (1,386 seconds), offering a mix of content lengths.

2. **Good Time Society:**
   - Slightly lower mean sentiment score (0.30), but still positive.
   - Moderate mean view count (8,220).
   - Longer mean duration (3,781 seconds), providing potentially more in-depth content.

3. **No Rolls Barred:**
   - Lower mean sentiment score (0.20), but still positive.
   - Highest mean view count (157,421), indicating popularity.
   - Longer mean duration (3,931 seconds), offering potentially more in-depth content.

Considering the preference for a positive atmosphere and moderate to high average view counts:

- **"Actualol"** aligns well with a positive atmosphere and a mix of content lengths.
- **"No Rolls Barred"** stands out for having the highest mean view count, though with a slightly lower positive sentiment score.
- **"Good Time Society"** has a positive atmosphere but a lower mean view count, which might be a downside.

Considering the updated preference for higher views:

- **No Rolls Barred** becomes a strong contender due to the highest mean view count with a moderate positive environment.
- **Actualol** remains a good choice for a strong positive atmosphere with a balanced mix of content.

## Conclusion <a name="conclusion"></a>

After exploring all these channels, I have decided to likely explore the channels **No Rolls Barred** & **Actualol**. Overall this was a fun side project, getting to practice retrieving data through API's and using data exploration skills on genre of board games

To explore the full code and analysis, please check the repo https://github.com/gavman95/youtube-boardgame-analysis/blob/ad731bf4425d52caa063d9a97008863ef5fabbc4/youtube%20analysis/youtube_boardgame_analysis.ipynb




