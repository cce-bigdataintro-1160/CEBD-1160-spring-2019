# Python Data Visualization

### Agenda
* Homework Check
* Visualizing data with Matplotlib
* Visualizing data with Seaborn
* About choosing the right plots
* Final Notes on Python Data Visualization
* Homework

### Python Data Visualization

##### Goals
Learn techniques for plotting different charts using numpy arrays and pandas dataframes. 
By the end of this class you'll be able to:
* Understand matplotlib basic objects: figures and axes
* Create simple line plots using matplotlib
* Save matplotlib pictures to a local directory
* Decorate and customize charts
* Perform visual exploration on datasets in order to extract insights
* Bring your plotting to the next level using seaborn
* Apply these techniques to your final project in order to answer your originally formulated question

##### Visualizing data with Matplotlib
* [matplotlib](https://matplotlib.org/index.html): Matplotlib official page
* [matplotlib Galleries](https://matplotlib.org/gallery/index.html): matplotlib Gallery with many plots to use for reference
* [Anatomy of a Figure](https://matplotlib.org/_images/anatomy.png): the anatomy of a matplotlib plot
* [matplotlib markers](https://matplotlib.org/api/markers_api.html): List of all markers available in matplotlib
* [matplotlib linestyles](https://matplotlib.org/gallery/lines_bars_and_markers/line_styles_reference.html): List of linestyles available in matplotlib

* It's possible to create plots in matplotlib using a few different syntaxes
* We can generate grids with multiple plots and arrange the layout in different ways
* Matplotlib supports displaying images with the `show()` command, saving them to files with `savefig()` or displaying them automatically on Jupyter notebooks
* Let's look at some [examples](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class6-notebook)
* The words columns, features and dimensions will be used interchangeably and mean the same thing!!!

1. Using the dataset you chose for your project. Plot one chart of each type:
  - `plot` passing one column(feature)
  - `plot` passing two columns(features)
  - `scatter` plot passing two columns(features)
2. Make sure to add a `title`, `xlabel` and `ylabel` on each of the previous plots
3. Put the the 3 plots above on the same figure and save it on a single file
4. Play with the `color`, `linestyle`, `linewidth`, `marker`, `alpha` parameters of a `scatter` plot. You don't need to use multiple charts per figure anymore, just one is fine.
5. Use one more feature(column) to play with the `size` parameter of a `scatter` plot
6. Do a multifeature plot! Plot 3+ `scatter` plots on the same `ax` comparing one variable to other columns at the same time. Make sure to add a `legend` to make your multifeature chart easier to read. 
7. Modify the previous chart to use the `size` and `color` parameters. Tip, the `size` can be based on one of the features!
8. Explore your dataset by plotting scatter plots comparing all columns 2 at a time. Tip, use nested for-loops for this!

##### Visualizing data with Seaborn
* [seaborn](https://seaborn.pydata.org/): Seaborn official page
* [seaborn Examples Gallery](https://seaborn.pydata.org/examples/index.html): gallery with examples for reference
* [matplotlib cmaps](https://matplotlib.org/tutorials/colors/colormaps.html): matplotlib color maps to customize the seaborn plots color scheme
* For all exercises below look at the references in the seaborn [class6-notebook](https://github.com/cce-bigdataintro-1160/spring2019/tree/master/class6-notebook)

1. Recreate one of the line plots you created in the previous exercise, now using `sns.lineplot`
2. Recreate one of the scatter plots you created in the previous exercise, now using `sns.scatterplot`
3. Recreate one of the scatter plots you created in the previous exercise, now using `sns.jointploy`
4. Create a distribution plot using `sns.distplot` using any feature.
5. Create a categorical plot using `sns.countplot` using a categorical feature.
6. Create a categorical plot using `sns.violinplot` using a categorical feature.
7. Create a correlation heatmap using `sns.heatmap`. Pass in the df.corr() to see the correlation heatmap for all of yours features!
8. Create the `sns.pairplot` for your entire dataset

##### About choosing the right plots
* [Chart Suggestions](./viz-files/Advanced Presentation by Design - Chart.pdf): Chart suggestions from Advanced Presentation by Design by Andre Abela
* [Chart Suggestions Simplified](./viz-files/Graph Cheat Sheet.pdf): Simplified version of the chart suggestions
* [Charting Trends](https://trends.google.com/trends/explore?date=2018-03-03%202019-05-18&geo=US&q=matplotlib,seaborn,plotly,ggplot): Trends on the utilisation of charting libs

* It's very important to plot accordingly to the data you want to display(different data means different plots) and the information you want to convey. The chart suggestions above might help deciding what plots to use.
* Another strategy is to generate as many plots as possible and from it visually derive the 'best' ones
* There's also a large set of possibitilies we can create by applying mathematical operations on our plots like summing, subtracting and multiplying column values.

##### Final Notes on Python Data Visualization
* One important aspect is realize the power of mastering the programatic generation of plots. One can write a generic plotter that can receive many different types of datasets and produce those many plots automatically.
* Other aspects that can be configured programatically are automation, frequency, scheduling among other customizations
* Producing plots with python allows for access to data that could be otherwise difficult to read (databases, apis, shared directories, etc). Using python also makes it easy to make those plots available through: email, webpages, saved files on shared disks, etc
* The scale of data python can process is much higher than that of regular "office tools" making it able to process datasets that couldn't be handled otherwise. Notice that depending on the amount of data some techniques would still be required to "bucket" or "stream" the data.
* Other highly recommended libraries are ggplot and plotly

### Optional homework(no need to submit)
* Read the machine learning introduction in: [this link](http://scipy-lectures.org/packages/scikit-learn/index.html#introduction-problem-settings), in particular, sections `3.6.1` to `3.6.5`. Don’t worry if this is a bit complex right now - it’ll really vary based on your math background.

### Recommended Readings
* [Visualization of Multi Dimensional data](https://towardsdatascience.com/the-art-of-effective-visualization-of-multi-dimensional-data-6c7202990c57): Excellent article about the challenges and solutions to visualize multi dimensional data
* [matplotlib Tutorials](https://matplotlib.org/tutorials/index.html): matplotlib Tutorials for Beginners, Itermediate and Advanced users
* [matplotlib Sample Plots](https://matplotlib.org/tutorials/introductory/sample_plots.html#sphx-glr-tutorials-introductory-sample-plots-py): Here you'll find a host of example plots with the code that generated them.
* [Plotly](https://plot.ly/python/): Plotly's Python graphing library makes interactive, publication-quality graphs online. 
* [Plotly Express](https://www.plotly.express/): A gallery displaying the simplified version of the plotly python library, meant to accelerate the usage of the library. 
* [ggplot](http://ggplot.yhathq.com/): ggplot is a plotting system for Python based on R's ggplot2
