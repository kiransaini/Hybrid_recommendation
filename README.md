# Hybrid_recommendation
A mixed hybrid model of collaborative filtering and content based recommendation
The dataset used is: Amazon Clothing, Shoes and Jewelry. Two datasets have been used: the items metadata and the 5-core ratings dataset. 
Dataset link: http://jmcauley.ucsd.edu/data/amazon/

The files perform the following functions:

D2v_final.model- Doc2Vec model trained on all textual information available in the item dataset using gensim library.

Item-latent-space-rep_keras_create_model.ipynb - This file is used to train an auto encoder model on 60000 images from our item dataset, test if the latent space representation of images obtained at the encoder layer is effective and store the model.

Item-latent-space-rep_load_create_model- This file is used to obtain the latent space representation of all images in our item dataset using the stored encoder model and store it as content profile in a csv file. 

Encoder2.h5- Stored encoder model

Item_vector_image3.csv: This file contains the latent space representation of item images as a vector of length 16.

Item_vector2.csv: This file contains the latent space representation of all item text information as a vector of length 15.

Recommendation_system_content_subset1: This file is used to run our hybrid content-based recommendation system on our first subset.

Recommendation_system_content_subset2: This file is used to run our hybrid content-based recommendation system on our second subset.

Recommendation_system_content_subset3: This file is used to run our hybrid content-based recommendation system on our third subset.

Recommendation system_EDA: This file contains exploratory data analysis of our dataset.

Item-latent-space-rep_doc2vec_create_model : This file is used to create a doc2vec model trained on all text information on items, test the effectiveness of the model created and store the model.

Item-latent-space-rep_doc2vec_load_model: This file is used to obtain the latent space representation of all text information of items in our item dataset using the stored doc2vec model and store it as content profile in a csv file. 

Neighborhood based recommendation_collaborative: This file is used to perform clustering of users and user-user collaborative filtering
