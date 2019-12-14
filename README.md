# EECS 731 The Oscars (Assignment # 07)


### Quick Note:
If you are interested in only looking at notebook, please access the notebook in **/notebooks/visualizations.ipynb**.

/notebooks: Contains the notebook of this assignment.

/data: Contains the data csv files (movies.csv, ratings.csv, tags.csv)

Also, some content of this assignment and my assignment # 03 (Weekend Movie Trip) notebook will be similar, as I have used the same datasets for both assignments.

### Objective:

Great stories and great visual effects

1. Set up a data science project structure in a new git repository in your GitHub account

2. Download any of the data sets from previous projects

3. Load the data set into panda data frames

4. Formulate one or two ideas on how storytelling and visualization would help describe the data set and establish additional value

5. Build three or more compelling visualizations

6. Document your process and results

7. Commit your notebook, source code, visualizations and other supporting files to the git repository in GitHub


### Datasets:

For this assignment, I took three datasets from the MovieLens Website (https://grouplens.org/datasets/movielens/), namely **Movies, Ratings, and Tags datasets**. First, we do exploratory analysis on each dataset separately, followed by cleaning and merging (those datasets into one) process (Data csv files are in /data/ directory of this repository).

### Process:

<ul>
<li>First I loaded and inspected the three data csv files (movies.csv, ratings.csv, tags.csv), so I can explore and combine MOVIES, RATINGS, and TAGS information from them for data exploration. (Please see the /notebooks/data_explorer.ipynb for more details)</li>
<li>Then, we merge the information from these data frames into a new data frame that contains MOVIES, THEIR RATINGS AND TAGS VECTORS.</li>
 <li>Once we have individiual Dataframes and the combined movie dataframe ready, we then draw interesting visualizations that can prove really helpful in getting valuable insights.</li>
 </ul>

*The process and results are detailed as follows, as well as in /notebooks/visualizations.ipynb notebook.*

### Discussion and Results:

First, we do exploratory analysis on each dataset separately, followed by cleaning and merging (those datasets into one) process. Then, we draw some compelling visualization from three individual dataframes (Movies, Ratings, Tags) as well as from combined/merged dataframe.

**Movies Dataset Analysis:**

![](figs/fig1u.png)

As shown above, the movies csv file contains total **9724** unique movies. Consequenly, from the table, it is evident that it provides movies names and their **genre**. We can use the **genre** and **title** features for data modeling or visualizaing great insights.

**Ratings Dataset Analysis**

![](figs/fig2u.png)


As seen above, **610** users participated in movie ratings for **9724** unique movies. This dataset also has timestamp that may be useful in time based analysis or modeling. But for this assignment, for merging process later, I dropped this feature being not useful (as part of **feautre engineering/cleaning process**).


**Tags Dataset Analysis**

![](figs/fig3u.png)


![](figs/fig4u.png)

The tag dataset csv file contains tags that are given by the users to different movies. As shown above, **1572 (out of total 9724)** movies have been given total **1460** tags or keywords by **58 (out of total 610)** unique and different users. The tag feature assigned to different movies can be used again for **drawing compelling visualizations**.

# Datsets Cleaning and Merging Process

Next, we are merging different datapoints into single dataset that can be used for further process (e.g. Data Modeling for classification, clustering or regression purpose).

First, we **merge** *movies* and *ratings* data frames based on common *movieId* feature, followed by merging the resultant table with tags table based on *movieId* and *userId* featues.


![](figs/fig5u.png)

As we can see that there are some NaN values in the resultant table. So, we **drop** rows with any NaN value.

![](figs/fig6u.png)


This final dataframe also has some interesting insights, as follows:

**Unique Users :  54**

**Unique Movies :  1464**

**Unique Tags :  1424**


Consequently, number of row are reduced from *1,02,695* to just *3,476* rows, but more cleaner and ready to be used by data visualization process.

# Compelling Visualizations using

1) First compelling visualization that will be helpful is to get **TOP 20 MOVIE TAGS**, as shown in the graph below. It will give us information about the dominant style of movies in the given movie datasets.


![](figs/fig4u.png)



# Conclusion

This was the basic data science assignment, but, I believe this was the **most important data science asignment**. Because data cleaning/ feature engineering process is vital before doing any data modeling stuff. As there is a famous term in data science and machine/deep learning community for importance of data pre-processing, i.e. GIGO (Garbage In, Garbage Out). So, in my opinion, this assingment was very important and useful for me to understand the baseics of data pre-processing. So, first we loaded three separate datasets, followed by merging them into a single table based on some common features/fields. Along the way, we also did cleaning/feature engineering on these tables e.g. Dropping NaN values.


# References

1) https://github.com/usajid/731_assign3
