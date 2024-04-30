<img src="https://mjconroy.com/wp-content/uploads/2023/04/ATU-Logo.png" width="250" height="150">




## Higher Diploma in Science: Computing-Data Analytics 2024
### Module: Principles of Data Analytics


# **Analysis of the Palmer Penguins Dataset**




***



## **Background:**

The Palmer Penguins dataset contains data relating to size measurements for three species of penguins, Adelie, Chinstrap and Gentoo.  The data was collected from three islands in the Palmer Archipelago, Antarctica from 2007-2009, as part of research carried out by Dr. Kristen Gormen  '_[Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins(Genus Pygoscelis)'](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0090081)_ in association with the Palmer Station Long Term Ecological Research Program. The Palmer Station is located on Anvers Island in the Antarctic Peninsula. 




<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
</head>
<body>

<table>
    <thead>
        <tr>
            <th>Adelie</th>
            <th>Chinstrap</th>
            <th>Gentoo</th>
        </tr>
    </thead>
    <tbody>
        <tr>            
        </tr>
        <!-- Extra row for images -->
        <tr>
            <td><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e3/Hope_Bay-2016-Trinity_Peninsula%E2%80%93Ad%C3%A9lie_penguin_%28Pygoscelis_adeliae%29_04.jpg/1200px-Hope_Bay-2016-Trinity_Peninsula%E2%80%93Ad%C3%A9lie_penguin_%28Pygoscelis_adeliae%29_04.jpg" alt="Adelie Penguin" height='300', width='200'></td>
            <td><img src="https://upload.wikimedia.org/wikipedia/commons/0/08/South_Shetland-2016-Deception_Island%E2%80%93Chinstrap_penguin_%28Pygoscelis_antarctica%29_04.jpg" height='300' width='200' alt="Chinstrap Penguin"></td>
            <td><img src="https://cdn.download.ams.birds.cornell.edu/api/v1/asset/115369831/1200" height='300' width='200'alt="Gentoo Penguin"></td>
        </tr>
    </tbody>
</table>

</body>
</html>








<br>

<img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Ant-pen_map_anvers.PNG" width='400' height='400'>
<br>

## **About the dataset:**

The [Palmer Penguins dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/penguins.csv) contains the data of 344 penguins from three species: Adelie, Chinstrap and Gentoo collected from three islands: Biscoe, Dream and Torgersen. 
There are 7 variables. 3 of which are categorical variables. These include species, island and sex. There are four numerical variables that represent the physical characteristics of the penguins. These include body mass(g), flipper length(mm), bill length(mm) and bill depth(mm). Each row represents a penguin, Each column represents a variable. 

Using python, the different variables were analyzed using various data structures and libraries such as pandas. Pandas is a python library built on top of NumPy for data manipulation and analysis. The main data structures in pandas include dataseries and dataFrames. A dataseries is a 1D array capable of holding any data type such as such as integers, floats, strings, objects. This is similar to Numpy arrays but can be used to access specific elements. A dataFrame is a 2D labelled data structure with columns of different data types, similar to a spreadsheet where each column represents a variable and each row represents an observation. In this analysis the dataset was loaded from the .csv file on the seaborn github repository into a dataFrame using pandas







***


## **Summary Statistics:**

The describe() function in pandas generates descriptive statistics of the dataframe. It gives a summary of the central tendency, disperson and shape of the distribution of the dataset. 


<img src="statistics1.png">
<img src="statistics2.png">

Observations:
-   Gentoo: Largest in body mass and flipper size with smallest bill depth 
- Adelie: Smallest in body mass and flipper size with smallest bill length 
-   Chinstrap: Longest bill length, close to Gentoo and highest bill depth, close to adelie 
-  Didnt observe significant differences in means or standard deviations in Adelie Penguins features across the three islands. 
-   Mean and median were close in all variables. slight difference in body mass for chinstrap and Gentoo penguins suggesting slight right skewedness.
- Std Deviation is high but consistent across species. Standard deviation is the measure of dispersion from the mean. 
-   Bimodal distributions for body mass of Adelie and Gentoo. Multimodal for Chinstrap penguins. 
-   Bimodal distribution for Chinstrap flipper length. Multimodal for Gentoo bill length. Bill depth: unimodal for all species





<br>



### Barchart:

<br>
 <img src="barchart.png" width='500' height='500'>
        

<br>The barchart shows the variations in body mass per species and islands. Each bar represents the average body mass of each species and sex of the penguins on a particular island. From observation of the barchart male penguins are larger than female penguins. Male and female Gentoo penguins show a notable difference in body mass in comparison to Adelie and Chinstrap penguins. Adelie and Chinstrap penguins are similar in size for both male and female penguins.No significant difference noted for body mass per island for Adelie penguins. Adelie is present on all three islands whereas as Chinstrap is present on Dream Island and Gentoo on Biscoe. 


### Histogram:


<img src="histogram.png" width='500' height='500'>

<br>

Histograms show the distribution of numerical data by grouping datapoints that lie within a range of values in to a bin.  The higher the bar the greater the frequency of values. The histogram shows the distribution of flipper length colored by species. Adelie and Chinstrap appear to overlap significantly while Gentoo can be seen to be easily distingusable from them due to having the largest flipper size. From the summary statistics, the median and the mean were the same for Adelie and Chinstrap and only differed by 1 for Gentoo. Chinstrap has two modes so therefore it is said to be bimodal while Adelie and Gentoo are unimodal. The histograms look symmetric, however a slight deviation of the curve noticed on Gentoo. The .skew() value for Gentoo was 0.4 suggesting distribution is slightly right skewed, maybe due to variation within the subgroups. The skew() for Adelie and Chinstrap is low at 0.1 each. The closer to 0 the distribution is thought to be more symmetric and normally distributed



## [**Correlation:**](https://en.wikipedia.org/wiki/Pearson_correlation_coefficient)

### Pairplot: 
<br><img src="pairplot.png" width='600' height='600'>
<br>
A pairplot is used to see if there is any relationships between two variables. 
The plots are in a scatterplot matrix format where the row name represents the x-axis and column name represents the y-axis. The main diagonal subplots are the histogram distributions for each variable. 

The main observations from the pairplot is that the Gentoo penguins are linearly separated from the Adelie and Chinstrap penguins in body mass vs bill depth and flipper length vs bill depth. The Adelie and Chinstrap appear more clustered together in most plots. The plot which appears to have the least amount of overlap between the three species combined is bill length vs bill depth.  There is a minimal amount of overlap seen for Gentoo penguins in flipper length and body mass with Adelie and Chinstrap but Gentoo can still be seen to form a clear cluster and have a good degree of separation. From the pairplot there seems to be a positive linear relationship between body mass and flipper length as the data points cluster around a straight line that slopes upwards from left to right, showing a consistent relationship between the two variables with all species combined. The correlation coefficient is 0.87 as can be seen on the correlation heatmap below, This result indicates a strong positive linear correlation. The most interesting relationships to study further would be body mass vs flipper length due to the strong correlation between the variables and bill length vs bill depth as they show the least overlap between the species. 


### Correlation Heatmap:

<br><img src="correlation heatmap.png" width="450" height="450">
<br>
<br>


### Scatterplot:
 
<br>

<img src="scatterplot1.png" height="400" width="600">


Scatterplots are used to identify correlations between two variables.
There is a strong positive correlation between body mass and flipper length. The correlation coefficient is 0.87 which is close to 1. The closer a value is to 1 the higher the correlation. The correlation coefficient indicates the strength and the direction of the linear relationship. A positive correlation suggests that as one variable increases the other variable tends to increase also. In this case as the body mass of the penguins increases the flipper length of the penguins also increases. The slope of the line is 50.1533 which means on average for every 1mm increase in flipper length the body mass of the penguins increases approximately 50.1533g. The slope represents the rate of change in the dependent variable (body mass) for a one unit change in the independent variable (flipper length). 






### Correlation Heatmap per Species:
<br><img src="correlation heatmap per species.png" width="500" height="500">



### Scatterplot of flipper length vs body mass per species:


<img src="scatterplot2.png" width="500" height="500"> 


When separated by species, the correlation coefficient values were lower than when all data was combined. The highest correlation coefficient is seen with Gentoo penguins at 0.71, while not as high as when all species are combined it still indicates a relatively strong positive relationship between the variables. There is significant overlap between Adelie and Chinstrap penguins while Gentoo is both larger in body mass and flipper length and forms a distinct cluster. Chinstrap had a correlation coefficient of 0.64 which suggests a moderately strong positive linear relationship. Adelie had the lowest correlation value at 0.46 which shows a weaker relationship between the variables than Gentoo or Chinstrap penguins. However a moderate positive relationship is still seen. 

### Scatterplots of flipper length vs body mass per species and sex:
<p float="left">
<img src="scatterplot3.png" width="300" height="300">
<img src="scatterplot4.png" width="300" height="300">
<img src="scatterplot5.png" width="300" height="300">
</p>


When separated based on species and sex, the correlation coefficient value was lower for penguins except Chinstrap males which gave a slightly higher correlation value of 0.66. Although the relationship is weaker between the variables a linear positive relationship is still seen. 


### Discussion:

The result shows that there is a strong positive correlation between body mass and flipper length. As body mass increases, flipper lengths tend to increase also. 
The stronger correlation coefficient observed when not separated based on sex or species could suggest a more consistent or stronger relationship between flipper length and body mass when considering all data points regardless of species or sex. Lower correlation coefficients could be due to outliers, smaller sample sizes or variation within the subsets. Analysing all data points together increases the sample size and may give a more accurate estimate of the overall relationship. Body mass naturally varies among individuals in a population due to genetics, diet, environment etc. From Dr. Gormens research the Adelie penguins foraging niche may have been affected more than Gentoo or Chinstrap penguins in the year with lower sea ice concentrations as they are sea ice obligate.    
While the penguins each have specific features that can identify their species, determining the gender of the penguin requires genetic testing via blood samples. Measurements such as, body mass, bill and flipper lengths would be less time consuming with lesser costs associated.  From the research by Dr. Gormen bill depth and body mass were the best predictors of sex for Gentoo penguins. Body mass and bill length best predictors of sex for Adelie penguins, while bill length and depth were strong predictors of sex for chinstrap penguins. The penguins were studied at the start of the nesting period so results can only be relevant for then. Flipper length was not a strong predictor of sex for any of the three species which could mean it is less under sexual selection compared to body mass, bill length and depth. Due to body mass varation throughout the yearly cycle, Bill length and depth may be the most promising features of the penguin for identification of gender. 







### References:
***

1. Horst A, Gormen K, _Palmer Archipelago Penguins Data in the palmerpenguins R Package - An Alternative to Anderson’s Irises._ https://allisonhorst.github.io/penguins_paper_distill/rjarticle/penguins.html

2. Gormen, K, 2014_Ecological Sexual Dimorphism and Environmental Variability within a Community of Antarctic Penguins(Genus Pygoscelis)(https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0090081)

