# Movie Recommendation System (Content-based)

<p align="left"> 
<a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a>
<a href="https://flask.palletsprojects.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/pocoo_flask/pocoo_flask-icon.svg" alt="flask" width="40" height="40"/> </a> 
<a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> 
<a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> 
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> 
</p>

## **Table of Contents**
  - [**Introduction**](#introduction)
  - [**Architecture**](#architecture)
  - [**Similarity Score**](#similarity-score)
  - [**How Cosine Similarity works**](#how-cosine-similarity-works)
  - [**How to run the project**](#how-to-run-the-project)
  - [**How to get the API key**](#how-to-get-the-api-key)
  - [**Sources of the datasets**](#sources-of-the-datasets)

## **Introduction**
Movie recommendation system is a content-based system in which recommendation of movie is done based on the similarity of its (movie) attributes. Using this type of recommender system, if a user watches one movie, similar movies are recommended.  For example, if a user watches a comedy movie starring Adam Sandler, the system will recommend them movies based on same genre (comedy) or same actor (Adam Sandler), or both. 

## **Architecture**

![Recommendation App](https://user-images.githubusercontent.com/36665975/168742738-5435cf76-1a42-4d87-94b4-999e5bfc48d3.png)

## **Similarity Score** 

   How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## **How Cosine Similarity works**?
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.

  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)
  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)

## **How to run the project**?

1. Clone using git clone command or download this repository to your pc.
2. Install all the libraries mentioned in the requirements.txt file. Using the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. 
4. Replace YOUR_API_KEY in line no. 15 and 29 of `static/recommend.js` file and save it.
5. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
6. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
7. Enjoy...

## **How to get the API key**?

Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.

### **Sources of the datasets**

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

