# Binge Watch - Movie Recommendation Website
## Submission for Microsoft Engage 2022 🌟

This website provides all the details of the requested movie such as overview, genre, release date, rating, runtime, top cast, reviews, recommended movies, etc. It is created using Collaborative Filtering (Website) and Content based Filtering (Jupyter Notebook).
<img width="1432" alt="Screen Shot 2022-05-29 at 12 19 51 PM" src="https://user-images.githubusercontent.com/83874474/170855983-bd54ff13-500d-4936-9177-10a6fce3fea0.png">
The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API.

### 📌 Table of Contents
* [Features](#features)
* [Tech Stack Used](#tech-stack)
* [Algorithm followed for the build](#algo)
* [Setup](#set-up)
* [Application flow](#usage)
* [Hosting](#hosting)
* [Challenges faced and learnings](#challenges)
* [Future Scope](#scope)
* [Resources](#resources)
* [Feature Requests](#feature-request)

<a id="features"></a>
## 🎇🚀 Features
- Simple and actionable UI
- Search engine with autocomplete predictions
- Provides information about Top cast of the movie
- Easy access to recommended movies
- Provides option to search for movie with genre of like 
- Optional option of year along with genre is available
- Offer ten movies with selected genre
- System applies sentiment analysis to categorize user comments
- Reviews are provided for the movie
- [Add more features](#feature-request)...


<a id="tech-stack"></a>
## 💻 Tech Stack Used
image of ppt
### Tools and Languages: 
<p align="left"> <a href="https://getbootstrap.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/><a href="https://heroku.com" target="_blank"> <img src="https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg" alt="heroku" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg"  alt="Javascript" width="40" height="40"</a><a href="https://www.python.org" target="_blank"> <img src="https://user-images.githubusercontent.com/83874474/170855800-1f5157c5-0b54-41ef-978f-153665bc8330.svg" alt="bootstrap" width="40" height="40"/> </a><a href="https://jupyter.org" target="_blank"> <img src="https://user-images.githubusercontent.com/83874474/170855823-dc78f536-4a68-419f-8422-28af4c42dc29.svg" alt="bootstrap" width="40" height="40"/> </a>  </p>

  
<a id="algo"></a>
## 🛠 Algorithm followed for the build
### KNN machine learning algorithm
The k-nearest neighbors (KNN) algorithm is a simple, easy-to-implement supervised machine learning algorithm that can be used to solve both classification and regression problems. It belongs to the supervised learning domain and finds intense application in pattern recognition, data mining and intrusion detection. It relies on labeled input data to learn a function that produces an appropriate output when given new unlabeled data. It is also called a ‘lazy learner algorithm’ because it does not learn from the training set immediately instead it stores the dataset and at the time of classification, it performs an action on the dataset. Recipes in Python to use KNN as classifier as well as regressor. The accuracy of k-NN is greater than other machine learning algorithms.
'Time Complexity': O(N * logN)
'Auxiliary Space': O(1) 
  
 ### Similarity Score : 
 How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each            other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
  
<a id="#set-up"></a>
## 📦 Setup  
### How to get the API key?
Create an account in https://www.themoviedb.org/, click on the `API` link from the left hand sidebar in your account settings and fill all the details to apply for API key. If you are asked for the website URL, just give "NA" if you don't have one. You will see the API key in your `API` sidebar once your request is approved.
  
## How to run the project?
1. Clone this repository to your local machine.
2. Install all the libraries mentioned in the [requirements.txt](https://github.com/Khushis01/Binge-Watch/blob/main/requirements.txt) file with the command `pip install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. (Refer the above section on how to get the API key)
3. Replace YOUR_API_KEY in **both** the places (line no. 15 and 29) of `static/recommend.js` file and hit save.
4. Open your terminal/command prompt from your project directory and run the file `main.py` by executing the command `python main.py`.
5. Click on the address link from the terminal and open in your browser.
6. Hurray! That's it.

<a id="usage"></a>
## 📖 Application flow
  
  
<a id="hosting"></a>
## ✅ Hosting
 Website is hosted at https://alogorithms-microsoftengage.herokuapp.com/
 To host the server on Heroku :

1. Sign up/Log in to Heroku.
2. Create a new app from the dashboard.
3. Install the Heroku CLI if you don't have it already and log into your account using the CLI.
4. Create a local git repository of this project and make a remote repository for Heroku.
5. Commit your code to the repo if not already done.(Make sure a Procfile of the server's entry point is present)
6. Push changes to the Heroku remote repository.
7. Server will be successfully deployed to Heroku.
  
  
  
<a id="challenges"></a>
## 💡 Challenges faced and learnings
  
  
<a id="scope"></a>
## 🚧 Future Scope
  
 
<a id="resources"></a>
## 📚 Resources
  ###Data Set Used 
1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)

