# IMDB Sentiment Analysis (Streamlit App)  
This project implements an IMDB Sentiment Analysis classifier using TF-IDF vectorization and a Naive Bayes model. The app is built with Streamlit to provide an interactive interface where users can upload datasets, train the model, view accuracy, visualize confusion matrices, and test custom reviews.  

## Features  
- Interactive Streamlit UI  
- Sidebar controls for test size and TF-IDF max features  
- Upload IMDB dataset in CSV format  
- Train a Naive Bayes classifier on movie reviews  
- Display model accuracy  
- Visualize confusion matrix with Seaborn heatmap  
- Input custom reviews and classify as Positive or Negative  

## Requirements  
Install dependencies with:  
`pip install -r requirements.txt`  

requirements.txt should contain:  
`streamlit`  
`pandas`  
`scikit-learn`  
`seaborn`  
`matplotlib`  
`numpy`  

## Usage  
Run the app with:  
`streamlit run app.py`  
Then open the provided local URL (usually http://localhost:8501) in your browser.  

## Example Dataset  
The dataset should contain two columns:  
- `review`: text of the movie review  
- `sentiment`: categorical label (`positive` or `negative`)  

Example:  
| review | sentiment |  
|--------|-----------|  
| The movie was fantastic and thrilling | positive |  
| The plot was dull and predictable | negative |  

## Notes  
- Sentiment labels are mapped to numeric values: positive = 1, negative = 0  
- TF-IDF vectorizer uses English stop words and configurable max features  
- Confusion matrix is displayed after training for performance evaluation  

## License  
MIT License  
