# YouTube-Video-Transcript-Summarizer
Software that allows efficient and smooth generation of video summaries using the web link of the video.

## Abstract
  The YouTube Video Transcript Summarizer is a Python-based software used to generate video summaries automatically. Currently, videos are watched completely to extract information. It will help extract video summaries automatically and also will be helpful for students of all fields to get the video summary instantly and save their precious time from searching and analyzing each video manually.
Video summarization is to generate a short summary of the content of a longer video document by selecting and presenting the most informative or exciting materials for potential users. The output summary is usually composed of a set of keyframes or video clips extracted from the original video with some editing process. The aim of video summarization is to speed up the browsing of an extensive collection of video data and achieve efficient access and representation of the video content. By watching the summary, users can make quick decisions on the usefulness of the video. Depending on applications and target users, evaluating a summary often involves usability studies to measure the content informativeness and quality of a summary.
          This application provides an efficient and reliable tool to generate and analyze YouTube Video summaries in a fast and effective manner.


## Application Requirements

### 1. Get transcript for a given video

In this milestone, we are going to utilize a Python API that allows you to get the transcripts/subtitles for a given YouTube video. It also works for automatically generated subtitles, supports translating subtitles, and does not require a headless browser, like other selenium-based solutions do.
Create a function that will accept YouTube video ID as an input parameter and return parsed full transcript as output.

### 2. Perform text summarization
Text summarization is the task of shortening long pieces of text into a concise summary that preserves key information content and overall meaning.
There are two different approaches that are widely used for text summarization:
● Extractive Summarization: This is where the model identifies the important sentences and phrases from the original text and only outputs those
● Abstractive Summarization: The model produces a completely different text that is shorter than the original, it generates new sentences in a new form, just like humans do. In this project, we will use transformers for this approach.

In this project, we will use Hugging Face's transformers library in Python to perform abstractive text summarization on the transcript obtained from the previous milestone.
● Create a function that will accept the YouTube transcript as an input
parameter and return the summarized transcript as output.
● Instantiate a tokenizer and a model from the checkpoint name. Summarization is usually done using an encoder-decoder model, such as Bart or T5.
● Define the transcript that should be summarized.
● Add the T5-specific prefix “summarize: “

### 3.Display Summarized transcript
We have provided a basic UI to enable users to interact and display the summarized text but there are some missing links that must be addressed.        
