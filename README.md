## 🚀Introduction

I developed a recommendation system that utilizes the power of transfer learning using ResNet-50 architecture along with Annoy an optimized K-Nearest Neighbours algorithm to deliver personalized recommendations based on user input. By performing feature extraction on a large dataset of over 45,000 images using transfer learning with ResNet-50, I was able to effectively analyze the image data. To identify the top 5 closest matches to a user's input, I implemented a similarity search approach using K-Nearest Neighbours, providing personalized fashion recommendations. The system is user-friendly and intuitive, and allows for accurate and effective analysis of image data.

This  recommendation system showcases the versatility and power of  transfer learning, similarity search, and convolutional neural networks (CNNs), providing a solid foundation for building larger and more comprehensive recommendation systems

##   💻 Cloth Similar Recommendation Engine : Proposed Methodology 

In this project, we propose a model that uses Convolutional Neural Network and the Nearest 
neighbour backed recommender. As shown in the figure Initially, the neural networks are trained and then 
an inventory is selected for generating recommendations and a database is created for the items in 
inventory. The nearest neighbour’s algorithm is used to find the most relevant products based on the 
input image and recommendations are generated.

![work-model](https://user-images.githubusercontent.com/89743011/170476738-cdfcd048-8bfd-450c-ad58-20ec025d5b7c.png)


## 📊Application Flow-Chart


To generate recommendations, our proposed approach uses Sklearn Nearest neighbours . This allows us to find the nearest neighbours for the 
given input image. The similarity measure used in this Project is the Cosine Similarity measure. The top 5 
recommendations are extracted from the database and their images are displayed.

![flow-chart](https://user-images.githubusercontent.com/89743011/170476148-5c472690-675b-4907-91c4-9b9804668f6f.png)


## Convolutional Neural Networks

- Convolutional Neural Network is a specialized neural network designed for visual data, such as images & videos. But CNNs also work well for non-image data (especially in NLP & text classification).
- Its concept is similar to that of a vanilla neural network (multilayer perceptron) – It follows the same general principle of forwarding & backward propagation.
  
- Once the data is pre-processed, the neural networks are trained, utilizing transfer learning 
  from ResNet50. More additional layers are added in the last layers that replace the architecture and 
  weights from ResNet50 in order to fine-tune the network model to serve the current issue. The figure
  shows the ResNet50 architecture.



![59954intro to CNN](https://user-images.githubusercontent.com/89743011/170827497-76197e3a-e1b7-4e69-b809-9d6d076100f0.jpg)



## Getting the inventory

The images from Kaggle Fashion Product Images Dataset. The 
inventory is then run through the neural networks to classify and generate embeddings and the output 
is then used to generate recommendations. 

### The Figure shows a sample set of inventory data

![dataset-cover](https://user-images.githubusercontent.com/89743011/170478150-9204c659-06a4-48bf-8420-5fee02a3c4d3.png)



## Experiment and results

The concept of Transfer learning is used to overcome the issues of the small size Fashion dataset. 
Therefore we pre-train the classification models on the DeepFashion dataset that consists of 44,441
garment images. The networks are trained and validated on the dataset taken. The training results 
show a great accuracy of the model with low error, loss and good f-score.




## Dataset Link

 - [Kaggle Dataset Big size 15 GB](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-dataset)

 - [Kaggle Dataset Small size 572 MB](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)




## Screenshots


### Outfits generated for the given input image

![Screenshot (107)](https://user-images.githubusercontent.com/89743011/170464638-15a88b15-fd4c-4ac6-9be5-13a72b0b31a1.png)



## Installation

Use pip to install the requirements.

~~~bash
pip install -r requirements.txt
~~~




## 📖Usage

To run the web server, simply execute streamlit with the main recommender app:

```bash
streamlit run main.py
```




## [Built With/Dependencies](dependencies)

- **OpenCV** - Open Source Computer Vision and Machine Learning software library
 
- **Tensorflow** - TensorFlow is an end-to-end open source platform for machine learning.

- **streamlit** - Streamlit is an open-source app framework for Machine Learning and Data Science teams. Create beautiful data apps in hours, not weeks.

- **pandas** - pandas is a fast, powerful, flexible and easy to use open source data analysis and manipulation tool, built on top of the Python programming language.

- **scikit-learn** - Scikit-learn is a free software machine learning library for the Python programming language.

- **opencv-python** - OpenCV is a huge open-source library for computer vision, machine learning, and image processing.



## 💡Challenges Faced and Learnings

- Had very basic knowledge of Deep Learning, so I spent quality time on learning the new concepts attached to Deep Learning for this project and then began the design-build process of cloth-similar.

- Setting the dependencies with proper version is the most critical. 

