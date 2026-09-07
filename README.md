# Social Media Sentiment Dashboard

## Member 3 – Data Processing, NLP and Analytics

This module is part of a Social Media Sentiment Dashboard developed for a nonprofit organization.

### Objective

The objective of this module is to collect social-media data, process it using Pandas, perform basic NLP preprocessing, analyze the data, and generate dashboard-ready statistics.

### Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* NLTK
* Scikit-learn
* Hugging Face Dataset API
* Google Colab

### Data Source

The social-media dataset is collected through the Hugging Face Dataset Server API.

The selected dataset configuration is `abusive-founta`. Therefore, the dataset labels should be interpreted according to the dataset's original classification task rather than automatically treating them as positive, neutral, or negative sentiment.

### Processing Pipeline

The processing workflow is:

Hugging Face API
↓
Pandas DataFrame
↓
Data Inspection
↓
Data Cleaning
↓
NLP Preprocessing
↓
Tokenization
↓
Stopword Removal
↓
Vocabulary Creation
↓
Integer Token Encoding
↓
Label Encoding
↓
Pandas Analytics
↓
Dashboard Metrics

### Main Features

1. Load social-media data from the Hugging Face API.
2. Convert API data into a Pandas DataFrame.
3. Inspect dataset structure and data types.
4. Detect missing values.
5. Detect and remove duplicate records.
6. Analyze label distribution.
7. Clean social-media text.
8. Tokenize text using NLTK.
9. Remove English stopwords.
10. Generate word-frequency statistics.
11. Create a vocabulary.
12. Convert words into integer indexes.
13. Encode classification labels.
14. Generate dashboard-ready statistics.
15. Perform ten validation and testing cases.

### Error Handling

The module checks for:

* Empty datasets
* Missing required columns
* Missing text values
* Duplicate records
* Invalid text values
* Missing NLP processing results

### Testing

Ten test cases were performed to verify:

* Dataset loading
* Required columns
* Missing values
* Duplicate detection
* Label availability
* Text cleaning
* Tokenization
* Vocabulary creation
* Integer encoding
* DataFrame integration

### Limitations

The selected dataset configuration is primarily intended for abusive-language classification. Its labels should not be interpreted as sentiment labels without additional processing. If the final dashboard requires positive, negative, and neutral sentiment, an additional sentiment-classification model should be applied to the text.

### Conclusion

The module provides a structured data-processing pipeline for social-media information using Pandas and basic NLP techniques. The resulting cleaned and analyzed data can be integrated with the dashboard component for visualization and further decision-making.
