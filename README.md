# Exploratory Data Analysis (EDA) of 4 Board Game Youtube Channels

## Table of Contents
1. [Introduction](#introduction)
   1.1 [Aims, Objectives, and Background](#aims-objectives-and-background)
2. [EDA & Insights](#eda-and-insights)
   2.1 [Video Metrics](#video-metrics)
   2.2 [Subscriber Count](#subscriber-count)
   2.3 [Upload Schedule](#upload-schedule)
   2.4 [Relationship of likes/comments vs view](#relationship-of-likes-comments-vs-view)
   2.5 [Sentiment Analysis](#sentiment-analysis)
   2.6 [Popular Themes](#popular-themes)
   2.7 [Inquiries in Comments](#inquiries-in-comments)
4. [Conclusion](#conclusion)

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


### Upload Schedule <a name="upload-schedule"></a>

From the below visualisation, its interesting to see the different variety in the upload schedule of diiferent channels. For example Actualol mostly uploads their videos on weekdays, especially on Wednesday being the peak and closely followed by Thursday. Barely any videos are uploaded on the weekend, with just a few on Sunday. For The Dice Tower its a bit different with there quite being of an even spread in which days videos are uploaded, for example Tuesday, Wednesday, Thursday, Friday & Saturday all have similar number of uploads in the channels history. This could be as a result of change of upload schedule over time with The Dice Tower first upload in the year 2014. On the other hand, No Rolls Barred is the most recent channel to be set up (in 2020) compared to the other 4, and its upload schedule is distinct, with the majority of uploads occuring on Tuesday & Saturday. Finally, for Good Time Society, most uploads occured on Tuesday and then history of uploads drop each day.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/f5611c61-b23f-47d3-bd96-2efb6da4e072)

### Relationship between number of likes or comments vs number of views views? <a name="relationship-of-likes-comments-vs-view"></a>

From the below observation, the next thing I wanted to explore was whether number of likes or comments correlate with how many views a video reaches. From the scatterplots below, it can be seen that the number of views is strongly correlated with the number of comments/ likes of the video. The more number of likes or comments in a video, likely the more views. This is expected as with a larger audience size, there is the tendency for more engagement in a video.
![image](https://github.com/gavman95/youtube-boardgame-analysis/assets/51774640/0344821e-8527-490f-aefc-01e3d698f301)

### Sentiment Analysis <a name="sentiment-analysis"></a>

<!-- Perform sentiment analysis on the comments section of videos. -->

### Popular Themes <a name="popular-themes"></a>

<!-- Identify popular themes in the videos using NLP techniques. -->

### Inquiries in Comments <a name="inquiries-in-comments"></a>

<!-- Explore and analyze the inquiries posed in the comment sections of the videos. -->

## Conclusion <a name="conclusion"></a>

After exploring these topics, my end goal would be to help identify the best 2 channels I preferably would follow.
