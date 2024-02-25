A retrieval chatbot that speaks like a character from a TV series. Character - Barney Stinson from "How I met your mother".

I used site this site to download transcript of the Episodes https://scriptmochi.com/tv-series/how-i-met-your-mother  

To prepare the dataset I used a TF-IDF vectorizer and a cosine similarity to establish whether questions and answers are corelated (where 0 - totaly not correlated and 2 - correlated strongly).

Then I trained a BI Encoder to answer questinos. A telegram bot https://t.me/Barneybot was created to interact with the model. I tried various tipes of extracting answers from the dataset - question-answer similarity, question-question similarity. Finally I prefered question-question similarity with some added noise. Telegram bot then chooses randomly from top-3 answers of the model. Telegram  bot is now offline, sreenshots of the conversation can be found in Images. 
To do: it seems that bot answers too randomly. It is neccesary to lower some of it, lower a random noise or randomness of the choosen answer. It can be corrected latter.
