# Advanced NLP-Based Amazon Review Analytics and Predictive Trend Forecasting System

## Project Description
This project aims to harness cutting-edge Natural Language Processing (NLP) and machine learning techniques to analyze Amazon product reviews, identify sentiment trends, and extract meaningful insights. Beyond analyzing past and present customer feedback, our system employs predictive analytics to forecast future product trends and customer preferences. This dual approach enables businesses to make informed decisions, tailoring products and services to meet consumer needs more effectively.

## Installation Instructions

### Prerequisites
- Python 3.8+
- Virtualenv (recommended for creating an isolated Python environment)
- Git (for version control and cloning the repository)

### Setup
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/malik-ma/MLOps-Semester-Project.git
   cd MLOps-Semester-Project
2. **Set Up a Python Virtual Environment (Optional but Recommended):**
   ```bash
   virtualenv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
3. **Install Required Python Libraries:**
   pip install -r requirements.txt
   
## Usage Guidelines

### Data Preprocessing
Before training the models, the data must be preprocessed. This involves cleaning the text, tokenizing, removing stop words, and other necessary steps to prepare the data for analysis.

1. Navigate to the `/scripts` directory:
   ```bash
   cd scripts
2. Run the preprocessing script to clean and prepare the data:
   ```bash
   python preprocess_data.py

### Training the Sentiment Analysis Model
After preprocessing, the next step is to train the sentiment analysis model to classify the reviews into positive or negative sentiments.

1. Return to root directory and run the training script located in the sentiment analysis model directory:
   ```bash
   python models/sentiment_analysis/train.py

### Aspect-Based Sentiment Analysis
The aspect-based sentiment analysis tool groups feedback into thematic buckets for each category of products to determine which features are popular, valued, and in need of improvement.
1. From the project root directory, run the trend forecasting script:
   ```bash
   python models/feature_analysis/analyze.py

### Continuous Model Retraining
To ensure the models stay accurate and relevant, they can be retrained periodically with new data collected through web scraping.
1. Run the data collection script to scrape and preprocess new reviews (ensure you have permission to scrape data from the web):
   ```bash
   python scripts/scrape_new_reviews.py

## Code Structure
| Directory                   | Description                                                                                   |
|-----------------------------|-----------------------------------------------------------------------------------------------|
| `/data`                     | Contains scripts for data preprocessing and cleaning. Includes a README for dataset details. |
| `/models`                   | Model definition files and training scripts. Split into subdirectories for organizational clarity. |
| `/models/sentiment_analysis`| Houses the sentiment analysis model, including training and evaluation scripts.               |
| `/models/aspect_analysis`   | Contains the aspect-based sentiment analysis model and related scripts.                          |
| `/notebooks`                | Jupyter notebooks for exploratory data analysis, model experiments, and visualizations.      |
| `/scripts`                  | Utility scripts for tasks such as web scraping, data transformation, and automated model retraining. |
| `/docs`                     | Documentation files including project proposal, design documents, and additional resources.  |
| `/tests`                    | Unit tests and integration tests to ensure code reliability and support CI practices.        |
| `/.github`                  | GitHub specific configurations, including workflows for GitHub Actions.                      |
| `README.md`                 | The project's main README file with essential project information, installation instructions, and usage guidelines. |


## Contributing

## License

## Acknowledgments

