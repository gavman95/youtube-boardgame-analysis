# Exploratory Data Analysis (EDA) of 4 Board Game Youtube Channels

## Table of Contents
1. [Introduction](#introduction)
   1.1 [Aims, Objectives, and Background](#aims-objectives-and-background)
2. [EDA & Insights](#eda-and-insights)
   2.1 [Video Metrics](#video-metrics)
   2.2 [Subscriber Count](#subscriber-count)
   2.3 [Upload Schedule](#upload-schedule)
   2.4 [Sentiment Analysis](#sentiment-analysis)
   2.5 [Popular Themes](#popular-themes)
   2.6 [Inquiries in Comments](#inquiries-in-comments)
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

<!-- Include analysis of video metrics such as likes, comments, and views. -->

### Subscriber Count <a name="subscriber-count"></a>

<!-- Just to get things started off, I wanted to create a plot of the channels and their subscribers count. As we can see, The Dice Tower is the most followed channel at 334K, followed by No Rolls Barred at 320K, then Actualol at 106K, with Good Time Society being the least followed out of the four channels at 58.1K.

```python
from matplotlib.ticker import FuncFormatter
# Create a function to format the y-axis labels in thousands
fig, axes = plt.subplots(figsize=(10,5))
ax = sns.barplot(x='channel_name', y='total_subscribers', data=stats.sort_values('total_subscribers', ascending=False))
ax.yaxis.set_major_formatter(FuncFormatter(lambda x, pos: '{:,.0f}'.format(x/1000) + 'K'))
plot = ax.set_xticklabels(ax.get_xticklabels(), rotation=90)
plt.show() -->

### Upload Schedule <a name="upload-schedule"></a>

<!-- Explore and analyze the upload schedule of each channel. -->

### Sentiment Analysis <a name="sentiment-analysis"></a>

<!-- Perform sentiment analysis on the comments section of videos. -->

### Popular Themes <a name="popular-themes"></a>

<!-- Identify popular themes in the videos using NLP techniques. -->

### Inquiries in Comments <a name="inquiries-in-comments"></a>

<!-- Explore and analyze the inquiries posed in the comment sections of the videos. -->

## Conclusion <a name="conclusion"></a>

After exploring these topics, my end goal would be to help identify the best 2 channels I preferably would follow.
