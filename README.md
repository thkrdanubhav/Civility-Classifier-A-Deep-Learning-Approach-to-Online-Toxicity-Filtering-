## About the Project

This project focuses on detecting hate or negative comments  in Reddit . We scraped data using the `praw` API, labeled the comments as either hate (`1`) or non-hate (`0`), and trained a hybrid model using RoBERTa embeddings followed by an LSTM layer. The final model achieved high accuracy and robust classification performance across both classes.


How It Works

1. **Data Collection**: Reddit data is collected using `praw`, the Python Reddit API Wrapper.
2. **Labeling**: Each comment is labeled manually as hate (`1`) or non-hate (`0`).
3. **Preprocessing**: Text is cleaned, tokenized, and fed into the RoBERTa tokenizer.
4. **Embedding Generation**: RoBERTa-base is used to convert text into contextual embeddings.
5. **Classification**:
   - An LSTM layer processes RoBERTa embeddings to capture sequential patterns.
   - A dense layer outputs binary predictions.
6. **Evaluation**: The model is evaluated using Accuracy, Precision, Recall, and F1-score.



 Dependencies Required

- `transformers`
- `torch`
- `sklearn`
- `pandas`
- `numpy`
- `praw`
- `matplotlib` (optional for visualizations)
- `seaborn` (optional for plots)
- `tqdm`

You can install all dependencies using:

```bash
pip install transformers torch scikit-learn pandas numpy praw matplotlib seaborn tqdm
