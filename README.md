# EECS 731: The Oscars (Assignment # 07)


### Quick Note:
If you are interested in only looking at notebook, please access the notebook in **/notebooks/visualizations.ipynb**.

/notebooks: Contains the notebook of this assignment.

/data: Contains the data csv file (historical_product_demand.csv)

Also, some content of this assignment and my assignment # 05 (World Wide Products Inc.) notebook will be similar, as I have used the same datasets for both assignments.

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

I used the given Forecasts for Product Demand dataset (https://www.kaggle.com/felixzhao/productdemandforecasting) for this Demand Forecasting modeling assignment. (Data csv file is in /data/historical_product_demand.csv).

### Process:

<ul>
<li>First, I loaded the given csv file into the Pandas Dataframe. (Please see the /notebooks/visualizations.ipynb for more details)</li>
<li>Then, I did feature engineering and cleaning process.</li>
 <li> Finally, we drew and analyzed four time-based compelling visualizations to get some insights about the given dataset products, and inferred some key facts from these graphs. Please refer to notebook for more details.These four analysis are also given below and are Weekly based, Monthly based and Years Weeks based trends.</li>
 </ul>

*The process and results are detailed as follows, as well as in /notebooks/visualizations.ipynb notebook.*

### Discussion and Results:

First, we do feature engineering and cleaning process.

The given dataset, once loaded into the dataframe, was as follows:

![](figs/fig0u.png)

Although we have **2,160** unique products, but to simplify the process, we limit the scope of our visualization process by focusing on one **most in-demand top** product. As from our analysis given in the notebook, we observed that the **product Product_1359 is the top product**, so we focus on it during this project and draw **four compelling visualizations** and infer some valuable and key insights from them about this product. 


# Compelling Visualizations and Story-telling

1) First compelling visualization that will be helpful is to get **TOP 20 MOVIE TAGS**, as shown in the graph below. It will give us information about the dominant style of movies in the given movie datasets.


![](figs/fig4u.png)



# Conclusion

**Story telling and the Data visualization** are the main and vital components that can be considered as the main objective of any data science based explorative analysis. In this project, I learnt about few ways to yield compelling visualizations that can be helpful in telling interesting and valuable story about the data. First e cleaned the datasets, followed by merging them into a single common dataframe. Then, using individual dataframes (Movies, Ratings, Tags) as well as combined/merged dataframe, we **obtained several compelling visuaizations to tell valuable story about the given datasets**.


# References

1) https://github.com/Usajid/731_assign5
