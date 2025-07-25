
# Text Emotion Classification

This repository contains a project focused on classifying human emotions from text using natural language processing (NLP) and machine learning techniques. It uses a dataset of real-life experiences labeled with different emotions to train a model capable of understanding emotional context in text.

## Dataset

The dataset used in this project is `textemotion.txt`, which contains sentences annotated with **one-hot encoded labels** representing one of the following **seven emotions**:

| Index | Emotion   |
|-------|-----------|
| 0     | Joy       |
| 1     | Fear      |
| 2     | Anger     |
| 3     | Sadness   |
| 4     | Disgust   |
| 5     | Shame     |
| 6     | Guilt     |

Each line in the dataset looks like this:
```
[ 0.  0.  0.  1.  0.  0.  0.] When my grandmother died.
```
This example corresponds to the **Sadness** emotion.

## Files

- `text emotion.ipynb`: Jupyter Notebook containing all code for preprocessing, training, and evaluation.
- `textemotion.txt`: Text dataset with emotional sentences and corresponding labels.

## Features

- Text preprocessing:
  - Lowercasing
  - Tokenization
  - Stopword removal
- Feature extraction using:
  - TF-IDF Vectorizer
  - CountVectorizer (optional)
- Emotion classification using machine learning models:
  - Naive Bayes
  - Logistic Regression
  - Random Forest
- Model evaluation using:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/text-emotion-classification.git
cd text-emotion-classification
```

### 2. Install Dependencies

Install necessary Python libraries using pip:

```bash
pip install numpy pandas scikit-learn matplotlib seaborn
```

Or if you have a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 3. Run the Notebook

Start Jupyter and open the notebook:

```bash
jupyter notebook "text emotion.ipynb"
```

Run all cells to train and evaluate the emotion classification model.

## Future Enhancements

- Use pre-trained word embeddings like **Word2Vec**, **GloVe**, or **FastText**
- Implement deep learning models like **LSTM** or **BERT**
- Build a real-time emotion detection web app using **Flask** or **Django**
- Perform multi-label classification (some experiences may evoke multiple emotions)

## Applications

- Mental health and emotion monitoring
- Sentiment and opinion mining
- Social media analytics
- Customer support and chatbot systems

## Contributing

Contributions, suggestions, and improvements are welcome!

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/awesome-feature`)
3. Commit your changes (`git commit -m 'Add awesome feature'`)
4. Push to the branch (`git push origin feature/awesome-feature`)
5. Open a pull request

## License

This project is open-source and available under the [MIT License](LICENSE).

## Contact

For any questions, reach out to the project maintainer via GitHub or open an issue in the repository.
