# Voice of Customer at Terminal21 Pattaya
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Terminal21Pattaya.jpg)
Ref. https://th.tripadvisor.com/Attraction_Review-g293919-d15266527-Reviews-Terminal_21_Pattaya-Pattaya_Chonburi_Province.html

# Details
This work uses Latent Dirichlet Allocation (LDA) algorithm to analyze data collected from comments of Terminal21 in Pattaya to know customers' opinions towards this department store.

# Python code and results
Import required libraries, enable interactive visualizations, suppress deprecation warnings, read a CSV file from a specified URL, and check dataset loaded from CSV file.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_001.png)

Generate a list of Thai stopwords, create a list of words removed from text data, combine the stopwords and removed words into a single list, then tokenize a sentence and return words separated by commas in a new 'Review_tokenized' column.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_002.png)

Take a list of tokenized documents, split each document into individual words, and then use Gensim to create a dictionary where words are mapped to unique integer IDs for further text analysis and modeling. After that convert tokenized documents into a Gensim corpus using a bag-of-words representation and calculate word frequencies for each document, resulting in a list of word-frequency tuples.
Then, configure parameters for LDA topic modeling, create an index-to-word dictionary, and run the LDA modeling algorithm on the given corpus with the specified settings to generate a topic model.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/a4248ca4f24e90eb295b6f38fa993cdee7e55a22/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_003.png)

The number of groups is randomly chosen from a range of high values, and the appropriate number of groups is 3. The first topic describes stores within the mall – this place is a modern and spacious department store comprising numerous shops and restaurants.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_004.png)

The second topic describes activities in the mall – There are many places creating for taking a photo, lots of restaurants for having a meal of which the price is not expensive, and a variety of products for shopping.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_005.png)

The third topic describes atmosphere in the mall – This department store composes of brand name shops, restaurants decorated with foreign scenes. So do restrooms. Besides, there are lots of parking lots.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_006.png)

Then, perform topic modeling using the Gensim library, specifically the Latent Dirichlet Allocation (LDA) algorithm, commonly used for analyzing text data and identifying topics within a collection of documents. Use a pre-trained LDA model to assign topics and probability scores to each row of text data in a DataFrame. The 'topics' column will contain the most dominant topic for each document, while the 'score' column will contain the corresponding probability score for that topic.
![Alt Text](https://github.com/ChawinTSR/MADT8101_Customer_Analytics/blob/d56b3f6ae22901ee0c5fc23cfda7889eab728130/05_Voice%20of%20Customer%20Analytics/Figures/Screenshot_007.png)
