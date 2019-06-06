# Projects & Applications of Data Science

### Agenda
* Homework Check
* Pandas Dataframes manipulation techniques
* Data cleanup and preparation for sklearn
* Where do I go from here?
* Final Project

##### Goals
Goal for today will be to review the topics above, discuss everything we learned so far and what can we do from here.
Oh, almost forgot! And kickoff the final project development!

##### Pandas DataFrames manipulation, cleanup and preparation
* A review of what we've [seen](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class5-notebook)
* Looking a few new DataFrame [operations](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class8-notebook)
  * Concatenating DataFrames
  * Renaming columns
  * Replacing values
  * Mapping values

##### Data cleanup and preparation for sklearn
* An [overview](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class8-notebook) of some important data preparation techniques :
  * Filling up missing data
  * Encoding categorical features with dummy variables
  * Producing numerical data from textual data
  * Dropping columns with small impact or that add 'noise' (not really correlated)
* This way we should have only numerical values for sklearn
* Don't hesitate to consult the material from previous classes to do the exercise!

* [Insurance Claim](https://www.kaggle.com/easonlai/sample-insurance-claim-prediction-dataset)
* [Top spotify tracks of 2018](https://www.kaggle.com/nadintamer/top-spotify-tracks-of-2018)
* [Heart Disease at UCI](https://www.kaggle.com/ronitf/heart-disease-uci)
* [Titanic Challenge](https://www.kaggle.com/c/titanic)

1. Choose one of the datasets above
2. Explore the dataset webpage, read the documentation and author's proposal
3. Load the dataset using pandas
4. Print the dataframe statistical summaries looking for:
  * Relevant variables
  * The dimensions of the dataset
  * Variables with empty values
  * Variables to be cleaned, corrected or enhanced
5. Ask at least one question you can answer by using the dataframe filtering through predicate like:
`df_name[df_name['Age'] > 30]`. For example, using the Spotify dataset try to find the 10 most `danceable` songs.
6. Use the method `df['my_column'].value_counts()` on a categorical column.
7. Check the correlation of the variables in your dataset!
8. Plot everything you need in order to understand this dataset and its correlations. You can use all the techniques we learned in the previous classes.
9. Finally, choose a variable to be used as target and run your classification or regression.
10. Check if your score is acceptable!



##### Where do I go from here?
* Well, this will depend a lot on where do you want to go :)
* A few more guided exercises to warmup: [Data Carpentry](https://datacarpentry.org/lessons/)
* A good starting point to develop ML skills: [Kaggle Getting Started Competitions](https://www.kaggle.com/competitions?sortBy=grouped&group=general&page=1&pageSize=20&category=gettingStarted)
* A more advanced challenge with unprocessed data [Montreal Open Data](http://donnees.ville.montreal.qc.ca/)
* [Other Datasets](https://github.com/awesomedata/awesome-public-datasets)
* Study other Computer Science topics like web development and microservices in order to deploy ML models
* [CCE Big Data Diploma](https://www.concordia.ca/cce/programs/big-data.html)

![](https://media.giphy.com/media/1n4FT4KRQkDvK0IO4X/giphy.gif?raw=true)

* [Reality will be more like](https://media.giphy.com/media/3o85xxSZvFZgD4wXde/giphy.gif) 
* ...but persist!!!



##### Final Project - to be presented on Saturday 15/06
* [Final project instructions/template](https://github.com/cce-bigdataintro-1160/cebd1160_project_template)
* [Final project example](https://github.com/cce-bigdataintro-1160/cebd1160_project_template/tree/gkexample)

* You may use the template structure to guide your thinking, but don't feel constrained by it, add and modify sections as you see fit
* Back your claims using plots and data obtained using your dataset analysis skills
* Make sure to add references for libraries and methods you're using  
* You can look for other people that "solved" your dataset on Google. You might find many ideas that you hadn't thought of!

* FAQ
  * Can I change my originally chosen dataset?
    
    Yes!

  * Can I change my originally chosen question?
    
    Yes too!

  * Can I change the csv dataset instead of the sklearn one?
    
    Yes, but take the risks into account, they haven't been 'prepared'!

  * How many plots should I add to my project?
    
    There isn't really a limit, try to stick with the "best" ones in order to explain each section of your template!

  * How do I format/style my project to look as good as the sample project?
    
    Look at the raw version of it [here](https://raw.githubusercontent.com/cce-bigdataintro-1160/cebd1160_project_template/gkexample/README.md)!!!

  * How long should my presentation be?
    
    5-10 minutes should be fine!  

  * Is there a specific algorithm I should use?
    
    You can use as many algorithms as you want and compare their results. Besides don't hesitate to try to optimize your score using feature selection or any other techniques you might find interesting!

  * I'm really stuck! I don't know exactly if my question is good or how to solve it...
    
    Google for inspiration! The reasons those datasets were chosen is because they've been largely used in Machine Learning literature. This means you'll find awesome inspiration around the internet, which I recommend you read and understand throughly to help you!  

### About 
* [How to show you master bigdata](https://pixelastic.github.io/pokemonorbigdata/)
* [Database Ranking](https://db-engines.com/en/ranking)
* [A ton of big data related technologies](https://github.com/onurakpolat/awesome-bigdata)
