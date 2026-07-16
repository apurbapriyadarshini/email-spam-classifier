# Email Spam Classifier

A machine learning mini-project that classifies email/SMS messages as **Spam** or **Ham (Not Spam)**, using a Bag of Words text representation and a Multinomial Naive Bayes classifier.

## Project Structure

| File                    | Description                                               |
|--------------------------|-------------------------------------------------------------|
| `spam_classifier.ipynb` | Main Jupyter notebook with full workflow and interactive demo |
| `spam_classifier.py`    | Standalone Python script version                            |
| `spam_dataset.csv`      | Labeled dataset (`text`, `label` columns)                   |
| `requirements.txt`      | Python dependencies                                          |
| `.gitignore`            | Standard ignore rules for Python/Jupyter projects           |

## Setup

```bash
git clone <your-repo-url>
cd <repo-folder>
pip install -r requirements.txt
```

## Usage

### Run the notebook (recommended — includes visualizations and an interactive demo)

```bash
jupyter notebook spam_classifier.ipynb
```

### Or run the plain script

```bash
python spam_classifier.py
```

## Methodology

1. **Data Loading** — The dataset is loaded from `spam_dataset.csv`.
2. **Exploratory Data Analysis** — Class distribution is visualized.
3. **Feature Extraction** — Text is converted to numerical vectors using `CountVectorizer` (Bag of Words).
4. **Train-Test Split** — The dataset is split into training and testing sets (75/25).
5. **Model Training** — A Multinomial Naive Bayes classifier is trained on the training set.
6. **Evaluation** — Accuracy, a classification report, and a confusion matrix are used to evaluate performance.
7. **Interactive Demo** — The notebook includes a live text box where any message can be typed in and classified in real time.

## Results

The model achieves approximately **85% accuracy** on the test set for this sample dataset.

## Future Improvements

- Use a larger, real-world dataset (e.g., the Kaggle SMS Spam Collection dataset)
- Apply TF-IDF vectorization instead of simple word counts
- Compare performance against other algorithms such as Logistic Regression or Support Vector Machines
- Add text preprocessing steps such as lemmatization and removal of punctuation/numbers

AI/ML Intern, CodTech IT Solutions InternID: CITS5467
