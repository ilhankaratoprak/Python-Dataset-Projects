# YouTube Video Analysis Project 
## Overview This project analyzes a dataset of YouTube videos to provide insights into various metrics such as views, likes, dislikes, and tags. The primary goal is to understand video performance by calculating the like-to-dislike ratio, tag counts, and other relevant statistics. 
## Dataset The dataset contains the following columns:
 - **video_id**: Unique identifier for each video. 
- **title**: Title of the video.
 - **channel_title**: Name of the channel that uploaded the video. 
- **category_id**: Category identifier for the video.
 - **publish_time**: Timestamp of when the video was published. 
- **tags**: List of tags associated with the video, separated by a pipe (`|`). 
- **views**: Total number of views the video has received. 
- **likes**: Total number of likes the video has received. 
- **dislikes**: Total number of dislikes the video has received. 
- **comment_count**: Total number of comments on the video.
 - **title_line**: The length of the video title. 
- **count_tags**: Number of tags associated with the video. 
- **likes_rates**: Calculated ratio of likes to the total of likes and dislikes. 
## Features 
1. **Tag Count**: Count the number of tags associated with each video. 
2. **Likes to Dislikes Ratio**: Calculate the ratio of likes to the total of likes and dislikes to gauge video reception. 
3. **Sorting Functionality**: Sort videos based on their likes rates to find the most positively received videos. 

## Installation You can install the required packages using pip: 
- pip install pandas numpy