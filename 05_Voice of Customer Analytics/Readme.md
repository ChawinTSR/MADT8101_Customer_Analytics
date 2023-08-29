# Abstract
xxx
# Voice of Customer at Terminal21 Pattaya
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Terminal21Pattaya.jpg)
Ref. https://th.tripadvisor.com/Attraction_Review-g293919-d15266527-Reviews-Terminal_21_Pattaya-Pattaya_Chonburi_Province.html

Import required libraries, enable interactive visualizations, suppress deprecation warnings, read a CSV file from a specified URL, and check dataset loaded from CSV file.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_001.png)

Generate a list of Thai stopwords, create a list of words removed from text data, combine the stopwords and removed words into a single list, then tokenize a sentence and return words separated by commas in a new 'Review_tokenized' column.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_002.png)

Take a list of tokenized documents, split each document into individual words, and then use Gensim to create a dictionary where words are mapped to unique integer IDs for further text analysis and modeling. After that convert tokenized documents into a Gensim corpus using a bag-of-words representation and calculate word frequencies for each document, resulting in a list of word-frequency tuples.
Then, configure parameters for LDA topic modeling, create an index-to-word dictionary, and run the LDA modeling algorithm on the given corpus with the specified settings to generate a topic model.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_003.png)

![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_004.png)

![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_005.png)

![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_006.png)

![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_007.png)
