2018 August

Netflix-Movie-Recommendation
===========================


---------------------------------------------------------------------------

Repository Overview:
--------------------



This project aims to build a model that Recommends Movies Netflix users based on User-User and Movie-Movie similarity.<br>
Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on<br>
the same training data set. (Accuracy is a measurement of how closely predicted ratings of movies match subsequent actual ratings.)
<br><br>
The repository has 1 ipython notebook.
<br>
1 [Netflix_Movie_2.ipynb](https://github.com/srvds/Netflix-Movie-Recommendation/blob/master/Netflix_Movie_2.ipynb)  
<br><br>
All the code is written in python 3 <br><br>
**DEPENDENCIES**
* tqdm
* numpy
* random
* pandas
* matplotlib
* seaborn
* sklearn
* scipy
* datetime
* xgboost
* surprise [About surprise library](http://surprise.readthedocs.io/en/stable/getting_started.html#load-dom-dataframe-py)     [Install surprise Library](https://github.com/NicolasHug/Surprise#installation)


Introduction:
-------------

Netflix is all about connecting people to the movies they love. To help customers find those movies, they developed world-class movie recommendation system: CinematchSM. Its job is to predict whether someone will enjoy a movie based on how much they liked or disliked other movies. Netflix use those predictions to make personal movie recommendations based on each customer’s unique tastes.

Netflix provided a lot of anonymous rating data, and a prediction accuracy bar that is 10% better than what Cinematch can do on the same training data set
<br>
For a given movie and user we need to predict the rating would be given by him/her to the movie. <br>
The given problem is a Recommendation problem <br>
It can also seen as a Regression problem <br>
<br>

This project tries many approaches and compares them

-----------------------------------------------------

Dataset:
--------

The dataset can be downloaded from
https://www.kaggle.com/netflix-inc/netflix-prize-data/data
<br><br>
<p> Data files : 
<ul> 
<li> combined_data_1.txt </li>
<li> combined_data_2.txt </li>
<li> combined_data_3.txt </li>
<li> combined_data_4.txt </li>
<li> movie_titles.csv </li>
</ul>
 
<br><br>
#### Understanding the dataset
The first line of each file [combined_data_1.txt, combined_data_2.txt, combined_data_3.txt, combined_data_4.txt] contains the movie id followed by a colon. Each subsequent line in the file corresponds to a rating from a customer and its date in the following format:

CustomerID,Rating,Date

MovieIDs range from 1 to 17770 sequentially.
CustomerIDs range from 1 to 2649429, with gaps. There are 480189 users.
Ratings are on a five star (integral) scale from 1 to 5.
Dates have the format YYYY-MM-DD.
#### Featurization
The four data files named combined_data_1.txt, combined_data_2.txt, combined_data_3.txt, combined_data_4.txt are Merged.
And whole data is formatted as: u_i:(user id i), m_j (movie id j), r_ij (rating of movie j by user i)

Many featurization and models are compared. The detailed documentation is in the Notebook.
 
-------------------------------------------------------------------------------

Analysis
--------

For detailed code of this section you can always check the Notebook.
<br>
#### Statistical Analysis<br>

count    1.004805e+08 <br>
mean     3.604290e+00 <br>
std      1.085219e+00 <br>
min      1.000000e+00 <br>
25%      3.000000e+00 <br>
50%      4.000000e+00 <br>
75%      4.000000e+00 <br>
max      5.000000e+00.<br>


References:
-----------

https://www.netflixprize.com/rules.html <br>
https://www.kaggle.com/netflix-inc/netflix-prize-data <br>
https://medium.com/netflix-techblog/netflix-recommendations-beyond-the-5-stars-part-1-55838468f429 <br>
http://surpriselib.com/ <br>
http://surprise.readthedocs.io/en/stable/getting_started.html <br>
https://github.com/NicolasHug/Surprise#installation <br>
http://courses.ischool.berkeley.edu/i290-dm/s11/SECURE/a1-koren.pdf <br>
https://www.youtube.com/watch?v=P5mlg91as1c <br>
https://appliedaicourse.com <br>


