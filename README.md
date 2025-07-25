# 🥗 NutriGuide

**NutriGuide** is an intelligent Indian recipe recommender system that uses Natural Language Processing and calorie-based filtering to suggest the most relevant recipes based on your available ingredients and dietary preferences.

---

## 🚀 Features

- 🧠 Ingredient extraction using SpaCy NLP
- 📊 TF-IDF vectorization + Cosine Similarity for content matching
- 🔢 Estimated calorie-based personalization
- 🌱 Diet filter (e.g., Vegan, Vegetarian, etc.)
- 📋 Clean, structured recipe output (tabular & HTML)

---

## 🧠 Technologies Used

- Python 3.x
- Pandas, NumPy
- SpaCy (`en_core_web_sm`)
- NLTK (Stopwords)
- Scikit-learn (TF-IDF, Cosine Similarity)
- Jupyter Notebook / Python scripts

---

## 📂 Dataset

- **File**: `IndianFoodDatasetCSV2.csv`
- **Source**: Public domain 
- **Key Fields**:
  - `TranslatedRecipeName`
  - `TranslatedIngredients`
  - `EstimatedCalories`
  - `Diet`
  - `TranslatedInstructions`

---

## 🧪 How to Run NutriGuide

### 1. Clone the Repository
```bash
git clone https://github.com/Nandita1001/NutriGuide.git
cd NutriGuide

# 🔧 Install Dependencies

Make sure you have Python 3.8+ installed, then run:

```bash
pip install -r requirements.txt
pip install spacy nltk
python -m spacy download en_core_web_sm

# Run the Recommender
user_ingredients = ["tomato", "onion", "pepper"]
diet = "Vegan"
recommend_recipes(user_ingredients, diet, calories=250, top_n=5)

