
#Project1
References
Stoll, J. (2023, October 2). SVOD service viewership shares in the U.S. 2023. Statista. https://www.statista.com/statistics/1412763/svod-service-viewership-share-us/#:~:text=In%20the%20first%20half%20of,playbacks%20through%20the%20Reelgood%20app. 

Links to Datasets
Shivam Bansal. Netflix Movies and TV Shows. Kaggle.
	https://www.kaggle.com/datasets/shivamb/netflix-shows/

Shivam Bansal. Hulu Movies and TV Shows. Kaggle.
	https://www.kaggle.com/datasets/shivamb/hulu-movies-and-tv-shows

Shivam Bansal. Disney+ Movies and TV Shows. Kaggle.
	https://www.kaggle.com/datasets/shivamb/disney-movies-and-tv-shows

Shivam Bansal. Amazon Prime Movies and TV Shows. Kaggle.
	https://www.kaggle.com/datasets/shivamb/amazon-prime-movies-and-tv-shows

Coding Resources
In the file named “Data_Compilation”:
The “pd.to_numeric”, which changes the values in the “Vote Average” column to floats was sourced from a Stack Overflow board, which can be found here: https://stackoverflow.com/questions/15891038/change-column-type-in-pandas.
It was used in Cells 5, 9, 14, 19, 22, 25, 30, 35.
The “.apply (lambda x:str(x).split(",")).tolist()” and the “...DF.stack()”, which unnest the values in the “Genre” and/or “Country” columns respectively, were sourced from Kaggle user who demonstrated an extensive dataset cleanup. It can be found here: https://www.kaggle.com/code/janiket3/netflix-data-cleaning-visualization-recommendation#Graphical-analysis.
It was used in Cells 6, 10, 15, 16, 20, 21, 23, 24, 26, 27, 31, 32, 36, 37.

In the file named “Streaming Service Analysis”:
The “plt.tight_layout()”, which ensured the axis labels wouldn’t be cut off when the figure was saved locally, was sourced from docs.kanaries.net, which can be found here: https://docs.kanaries.net/topics/Matplotlib/matplotlib-savefig-cuts-off-labels. 
It was used to produce all of the charts within the first 18 cells in the file. 

Under the “Question To Be Answered: What is the overall quality of content on the streaming service based on viewer ratings (Vote Average)?” 
For Prime, Disney, and Netflix sections, the “pd.concat()” method was used to stack the movies and TV shows DataFrames for each of the streaming services (i.e., append the rows of the TV Shows DataFrame under the movies DataFrame)

Code reference: https://www.geeksforgeeks.org/how-to-stack-multiple-pandas-dataframes/

Under the “Box Plot Charts - All Content” section: the “medianprops”, “boxprops” and “ax = df[].plot()” were used to prepare the box plots in one figure, including chart colors and styles

Code reference:
medianprops: https://matplotlib.org/stable/gallery/statistics/boxplot.html
boxprops: https://matplotlib.org/stable/gallery/statistics/boxplot.html
Box Plots in same figure: https://www.tutorialspoint.com/plot-multiple-boxplots-in-one-graph-in-pandas-or-matplotlib


Used code from  https://matplotlib.org/stable/gallery/lines_bars_and_markers/barchart.html and https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.bar.html#matplotlib.axes.Axes.bar to create a grouped bar chart
Used in cell 11

Used  code (bbox_to_anchor=()) from https://matplotlib.org/stable/gallery/pie_and_polar_charts/pie_and_donut_labels.html# to adjust location of legends
Used in cells 22, 32, 42, 52
