## Product Recommendation System Based on Amazon Review

## Overview

This project develops a **Product Recommendation System** that predicts user ratings and evaluates review usefulness based on the **Amazon Review Electronics Dataset**. Using collaborative filtering techniques and natural language processing (NLP), the system recommends relevant products to users, enhancing personalization and engagement.

## Features

- Predict user ratings using machine learning models.
- Preprocess and analyze review text using NLP techniques.
- Perform exploratory data analysis (EDA) to uncover trends and insights.
- Build a collaborative filtering-based recommendation system (User-User and Item-Item).
- Evaluate model performance with detailed metrics.

## Dataset

The dataset used for this project is the **Amazon Electronics 5-core Dataset**, available [here](https://nijianmo.github.io/amazon/index.html). It includes product metadata and user reviews.

## Requirements

### Python Packages:

- pandas
- numpy
- sklearn
- nltk
- matplotlib
- seaborn
- wordcloud
- BeautifulSoup4

### Additional Setup:

- Install `nltk` resources:
  ```python
  import nltk
  nltk.download('wordnet')
  nltk.download('punkt')
  ```
- Data files:
  - `Electronics_5.json.gz`: User reviews.
  - `meta_Electronics.json.gz`: Metadata.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/NitishKumar1123/Product-Recommendation-System-Based-on-Amazon-Review.git
   cd Product-Recommendation-System-Based-on-Amazon-Review
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Place the dataset files in the project directory.

## Usage

1. **Data Preprocessing**:

   - Load and clean the dataset.
   - Preprocess text by removing HTML tags, special characters, and performing lemmatization.

2. **Exploratory Data Analysis**:

   - Generate descriptive statistics.
   - Visualize trends (e.g., word clouds, pie charts).

3. **Feature Engineering**:

   - Transform review text using Bag of Words (BoW), TF-IDF, and Hashing Vectorizer.

4. **Machine Learning Models**:

   - Train and evaluate models like Logistic Regression, Naive Bayes, and SVM.
   - Split data into training and testing sets (75:25).

5. **Collaborative Filtering**:

   - Build User-User and Item-Item recommendation systems.
   - Evaluate performance using MAE for different numbers of neighbors (N).

## Results

### Key Insights:

- **Best Performing Model**: Logistic Regression with an accuracy of **88%**.
- **Top Brands**: Sony, Sennheiser, and Audio-Technica.
- **Collaborative Filtering**: Effective for personalized recommendations.

### Recommendations:

The system identifies top products for users based on historical reviews and predicts ratings for unrated items.

## Directory Structure

```
Product-Recommendation-System-Based-on-Amazon-Review/
├── data/                 # Raw and processed datasets
├── Amazon_Product_Recommendation_System.ipynb            # Jupyter notebooks for experimentation
├── results/              # Outputs (plots, evaluation metrics, etc.)
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies
```

## Example Plots

- **Word Cloud**:
  Displays commonly used words in positive and negative reviews.
- **Pie Chart**:
  Shows distribution of ratings.
- **Trends Over Time**:
  Yearly count of reviews.

## Contributing

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Amazon for the dataset.
- Scikit-learn and NLTK for robust libraries supporting NLP and machine learning.

## Contact

For questions or feedback, contact **Nitish Kumar** at [nitish23129@iiitd.ac.in.com].
