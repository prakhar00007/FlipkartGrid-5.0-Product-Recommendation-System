
# ** Flipkart Grid 2023 Product Recommendation System**

This is a content-based product recommendation system that suggests similar products to a given product.




## **How it works**
The system works by analyzing the product metadata - name, description, brand, categories etc - and extracting keywords from this text data. The keywords are used to calculate similarity between products using TF-IDF vectors and cosine similarity. Products that are textually similar based on the metadata are recommended.

Additional filters can be applied like:

- **Price range**
- **Minimum discount percentage**

This helps narrow down the results and suggest products that are affordable and have good deals.

## **Data Preprocessing**

The product metadata is preprocessed to extract clean text for generating keywords. This involves:

- **Converting category hierarchy into separate words**
- **Removing stopwords, punctuations**
- **Lemmatization to reduce words to root form**

The preprocessed text is combined into a single column to represent the entire product metadata.

## **Similarity Calculation**

TF-IDF vectorizer is used to convert the preprocessed text into feature vectors. Cosine similarity is then calculated between these vectors to quantify similarity.
## **Recommendations**

For a given product, the most similar products based on cosine similarity are retrieved. Additional filters like price and discount percentage can be applied to filter the recommendations further.
## **Usage**

The main functions for using the recommendation system are:

- **`get_recommendations(product_name)`** - recommends similar products without any filters

- **`get_recommendations2(product_name, min_price, max_price)`** - recommends products in given price range

- **`get_recommendations3(product_name, min_price, max_price, min_discount)`** - recommends products in price range with minimum discount % filter

Here is an additional section in the README for including a PPT:

## **Presentation**
Here is an additional section including a PPT:
[Personalized-Product-Recommendations.pptx](https://github.com/Ankit-005/Product-Recommendation-System/files/12388108/Personalized-Product-Recommendations.pptx)


  
