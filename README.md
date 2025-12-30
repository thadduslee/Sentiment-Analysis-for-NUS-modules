# Sentiment-Analysis-for-NUS-modules
NUS Module Sentiment Analyzer
Automating the university module selection process using Long Short-Term Memory (LSTM) networks.

📖 Overview
Choosing university modules often leads to information overload, with students having to sift through hundreds of mixed reviews on platforms like NUSMods. This project solves that "analysis paralysis" by using Natural Language Processing (NLP) to aggregate comments and generate a clear, quantifiable sentiment score for each module.

🛠️ The Solution
Instead of manually reading reviews, this tool:

Scrapes module data and comments via API.

Cleans & Filters the data to isolate relevant user feedback.

Analyzes the text using a trained Deep Learning model.

Outputs an average sentiment rating (1-5 scale) for the module.

🧠 Model Architecture: Why LSTMs?
I chose LSTMs (Long Short-Term Memory networks) over traditional RNNs for this specific task.

Long-Range Dependencies: Student reviews often contain context where the sentiment depends on words far apart in the sentence. LSTMs maintain a "memory cell" that captures this context better than standard RNNs.

Gradient Stability: LSTMs effectively mitigate the vanishing and exploding gradient problems common in deep sequence models.

📊 Dataset Strategy
Due to the scarcity of labeled university-specific datasets, I utilized a Coursera Reviews Dataset (Kaggle) for training. The writing style and rating system (1-5 stars) closely mirror university module reviews, allowing for effective transfer of the learned sentiment patterns.

🚀 Tech Stack
Python

TensorFlow / Keras (LSTM implementation)

Pandas & NumPy (Data manipulation)

Requests (API Scraping)
