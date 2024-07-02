# YouTube-Sentiment-Analysis

## Project Overview
This project aims to analyze YouTube comments to understand user sentiment and engagement. The analysis includes sentiment polarity, word cloud visualization, emoji usage, category popularity, and the impact of punctuations on engagement metrics.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Analysis Details](#analysis-details)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Features
- Sentiment analysis using TextBlob
- Word cloud visualization for positive and negative comments
- Emoji analysis
- Category popularity analysis
- Audience engagement metrics (like rate, dislike rate, comment rate)
- Impact of punctuations on views, likes, and comments

## Installation
To get started with this project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/Nithya-15/youtube-sentiment-engagement-analysis.git
    cd youtube-sentiment-analysis
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

3. (Optional) Install additional dependencies for Colab:
    ```sh
    pip install google-colab
    ```

## Usage
1. Mount your Google Drive to access the dataset:
    ```python
    from google.colab import drive
    drive.mount('/content/drive')
    ```

2. Read the CSV file containing YouTube comments:
    ```python
    comments = pd.read_csv('/content/drive/MyDrive/UScomments.csv', on_bad_lines='skip')
    ```

3. Run the analysis scripts provided in the `youtube_analysis_shan_singh.ipynb` notebook.

## Dataset
The dataset used in this project includes YouTube comments and additional data files. Make sure to upload these files to your Google Drive in the specified directory:
- `UScomments.csv`
- `additional_data/US_category_id.json`
- Other CSV files in the `additional_data` directory

## Analysis Details
- **Sentiment Analysis**: Calculating polarity scores for comments using TextBlob.
- **Wordcloud Analysis**: Visualizing the most frequent words in positive and negative comments.
- **Emoji Analysis**: Extracting and counting the most used emojis in comments.
- **Category Analysis**: Identifying the most liked categories using YouTube category IDs.
- **Audience Engagement**: Calculating like rate, dislike rate, and comment rate for each category.
- **Punctuation Impact**: Analyzing the effect of punctuations on views, likes, and comments.

## Results
Key findings from the analysis include:
- Positive comments frequently mention words like "best", "awesome", "perfect".
- Negative comments emphasize words like "terrible", "worst", "boring".
- Emojis commonly used include "😂", "❤️", and "👍".
- Certain categories show higher engagement rates.

## Contributing
Contributions are welcome! Please create an issue or submit a pull request for any changes or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
- [TextBlob](https://textblob.readthedocs.io/)
- [WordCloud](https://github.com/amueller/word_cloud)
- [emoji](https://github.com/carpedm20/emoji)
- [Plotly](https://plotly.com/)
- [Seaborn](https://seaborn.pydata.org/)
