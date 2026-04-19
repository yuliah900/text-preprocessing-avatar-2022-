**Twitter Data Scraping & Text Preprocessing: Avatar The Last Airbender**
Academic Project | Data Mining & Natural Language Processing

📌 Project Overview
This project focuses on the end-to-end pipeline of handling unstructured social media data. It covers the process from automated data acquisition using Node.js to advanced text preprocessing, ensuring the dataset is clean and ready for statistical analysis or sentiment modeling.

🛠️ Tech Stack
- Environment: Google Colab, Node.js

- Tools: tweet-harvest (for automated scraping)

- Libraries: Pandas, NLTK, Regex (Regular Expressions)

🔍 Methodology
1. Data Acquisition (Automated Scraping)
Due to current API limitations, I implemented a workaround using Node.js and the tweet-harvest library to collect public discourse on X (Twitter).

  - Process: Configured a Linux-based environment in Colab to execute automated crawling.

  - Result: Successfully retrieved 1,507 raw tweets using the keyword "avatar the last airbender" (Indonesian language).

2. Advanced Text Preprocessing
Social media data is inherently noisy. I developed a multi-stage cleaning pipeline to ensure data quality:

  - Text Cleaning: Removed URLs, usernames (@), HTML elements, punctuation, and excessive whitespace.

  - Noise Removal: Specifically filtered out emojis, emoticons, and hashtags to focus on the core textual sentiment.

  - Deduplication: Identified and removed duplicate entries, refining the dataset from 1,507 to 1,353 unique records.

  - Tokenization: Segmented sentences into individual tokens for granular analysis.

3. Feature Selection & Refinement
To optimize the dataset for further analysis, I applied several NLP techniques:

  - Stopwords Removal: Filtered out common non-informative words.

  - Lemmatization: Reduced words to their base dictionary form to ensure consistency.

  - Data Structuring: Removed irrelevant columns and exported the final processed dataset into a clean CSV format.
