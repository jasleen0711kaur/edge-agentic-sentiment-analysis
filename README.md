# edge-agentic-sentiment-analysis
This is a fun project aimed at figuring out what needs to change for Edge to be PERCEIVED as a good agentic browser. This was done by figuring out how users feel and what they are feeling about different traditional and agentic browsers. For example, Perplexity = AI, Google Chrome = Bloat, etc. For tech geeks, it was done using pythong scripts to get Reddit posts using praw Python API, VaderSentimentAnalyzer, POS tagging and TF-IDF. This is what it means:
1. **Reddit comments scraping**: Get quality data.
Topic -> Microsoft Edge
Title -> Just moved to Edge and Bing from Chrome and I think that (maybe) MS has done a great job

2. **VaderSentimentAnalysis**: Check if the post is a positive/ neutral/ negative post.
<img width="461" alt="step3" src="https://github.com/user-attachments/assets/867af2df-9478-422e-8744-eed71c2b69f9" />

3. **POS**(Parts of Speech) tagging and **TF-IDF**(Term frequency- Inverse Document Frequency):  Use POS tagging to get nouuns and adjectives from that post. TF-IDF scoring helps identify how important isthat word for that particular broser/theme. High TF-IDF score means "This word appears a lot in this topic AND doesn’t appear much in other topics."
<img width="517" alt="step5" src="https://github.com/user-attachments/assets/95e7b328-ae42-4204-86f4-b6e7e2b7e299" />

Here's what the process of Sentiment analysis looked like:
1. Fetched 250 posts on multiple browsers but got only 860 quality posts.
2. Cleaned data to remove URLs, punctuation, etc.
3. Used VaderSentimentAnalyzer to map a sentiment score and label to each post.
🧠 At this point, you know how users feel — but not what they're feeling about. 
4. Extract the top distinctive keywords per browser by applying POS tagging and TF-IDF.
5. Assign themes to keywords and tracks how often each appears in positive, negative, or neutral posts per browser.
6. Add up how people feel (positive/negative) about each theme (like AI or Privacy) for every browser (like Edge or Chrome) to create an easy-to-compare summary table.
🧠 At this point, you know how people feel about each key theme (like AI or Privacy) for each browser. 
7. Make easy-to-read visuals that show what people like or dislike about each browser (like Edge or Chrome) across different areas like AI, Privacy, or Speed.

Scripts and data folder will help in a better understanding. Feel free to download the scripts from project_scripts and modify according to your needs. Happy learning!



