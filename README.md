# YouTube Video Summarizer

## Overview
The YouTube Video Summarizer is a web application that allows users to summarize YouTube videos by extracting and condensing the video transcript. Using advanced NLP techniques and models, the application provides a quick overview of video content, saving time for users.

![Screenshot 2024-10-30 142734](https://github.com/user-attachments/assets/4fdf2de9-2d83-422d-b440-0b562e6cba1f)

## Features
**Easy to Use**: Simply enter the URL of any YouTube video, and receive a summarized version of its transcript.
**NLP Powered**: Utilizes state-of-the-art models from the Hugging Face Transformers library to generate summaries.
**Flask Web Framework**: Built on Flask, making it lightweight and easy to deploy.
## Demo
Here’s a demonstration of the application in action:

https://github.com/user-attachments/assets/d51b3395-97f3-44a0-ae65-143ad251127e

## Technologies Used
**Flask**: For building the web application.

**YouTube Transcript API**: To extract video transcripts.

**Transformers**: For natural language processing and summarization.

**PyTorch**: For model implementation and execution.

## Code Explanation
The application is structured around a simple Flask web server. Here’s a brief overview of the main components:

**get_yt_transcript(url)**: Extracts the transcript from a YouTube video using its URL.

**get_summary(transcript, chunk_size=512)**: Splits the transcript into manageable chunks and generates a summary using a pre-trained T5 model.

**Flask Routes**:

"/": Renders the home page where users can input the YouTube video URL.

"/" (POST): Processes the input URL, retrieves the transcript, generates the summary, and returns it.
