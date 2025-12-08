Assignemnt 1
# infosys-springboard
Python OOP demonstrating Encapsulation, Inheritance, Polymorphism, Abstraction using Bank Accounts.

## Files
- `bank_oop.py` – Main Python file with:
  - `Account` (base class)
  - `SavingsAccount` (inherits from Account)
  - `PremiumAccount` (inherits from SavingsAccount)
## How to Run
1. Install Python (if not already installed).
2. Download or clone this repository.
3. Run the file:
4. Check the console output to see deposits, withdrawals, interest, and credit limit behavior.

## OOP Concepts Used
- **Encapsulation** – Balance and account details stored in protected attributes.
- **Inheritance** – SavingsAccount and PremiumAccount extend the base Account.
- **Polymorphism** – `withdraw()` behaves differently in each account type.
- **Abstraction** – Methods like `add_interest()` and `get_balance()` hide internal details.

Assignment 2
### Assignment 2 – Text Classification (Count vs TF–IDF vs Word2Vec)

File: `assignment2_text_models.ipynb
- Task: Compare performances of different text representations on a 10k tweet sentiment dataset (`train-processed-sample.csv` from Kaggle).
- Vectorizers:
  - `CountVectorizer` with `ngram_range=(1, 3)`
  - `TfidfVectorizer` with `ngram_range=(1, 3)`
  - Word2Vec averaged embeddings (using `gensim` Word2Vec model)
- Models:
  - `LogisticRegression`
  - `MultinomialNB` (used with Count/TF–IDF; not with Word2Vec)

**Main experiments**
1. Train Logistic Regression and MultinomialNB with:
   - CountVectorizer (1–3 grams)
   - TfidfVectorizer (1–3 grams)
2. Train Logistic Regression with Word2Vec averaged document vectors.
3. Observe:
   - Feature explosion and possible overfitting when using 1–3 gram n‑grams.
   - Differences in accuracy between Count, TF–IDF, and Word2Vec.

**Hyperparameter tuning with GridSearchCV**
- Tune `C` for `LogisticRegression` using TF–IDF features.
- Tune `alpha` for `MultinomialNB` using CountVectorizer features.
- Report:
  - Best `C` and cross‑validation accuracy for Logistic Regression.
  - Best `alpha` and cross‑validation accuracy for MultinomialNB.
  - Test accuracy of the best models.

**How to run**
1. Open `assignment2_text_models.ipynb` in Google Colab or Jupyter.
2. Make sure the dataset CSV (`train-processed-sample.csv`) is available at `/content/` (in Colab) or in the same folder (in Jupyter).
3. Run all cells from top to bottom:
   - Data loading and preprocessing
   - Vectorization (Count, TF–IDF, Word2Vec)
   - Model training and evaluation
   - GridSearchCV tuning
   - 
## Technologies Used
- Python 3
- scikit-learn (vectorizers, models, GridSearchCV)
- gensim (Word2Vec)
- pandas, numpy
- Google Colab / Jupyter Notebook

