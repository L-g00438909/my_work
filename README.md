<img src="https://mjconroy.com/wp-content/uploads/2023/04/ATU-Logo.png" width="250" height="150">




# Higher Diploma in Science: Computing-Data Analytics 2024
### Module: Principles of Data Analytics


# **Analysis of the Palmer Penguins Dataset**




<img src="https://allisonhorst.github.io/palmerpenguins/reference/figures/lter_penguins.png" alt="penguins" width="500"/> _Artwork by @Allison_Horst_
***


*Create a GitHub repository with a README.md and a .gitignore. Add a Jupyter notebook called penguins.ipynb and add a title to it.
Find the palmerpenguins data set online and load it into your Jupyter notebook. In your notebook, give an overview of the data set and the variables it contains.
Suggest the types of variables that should be used to model the variables in the data set in Python, explaining your rationale.
Create a bar chart of an appropriate variable in the data set. Then create a histogram of an appropriate variable in the data set.*

*Select two variables from the data set and provide an analysis of how correlated they are.*


### Introduction:
***

There are seven variables. There are three species found on three islands that are part of the Palmer Archipelago in Antarctica. the other 4 variables are numeric and they describe the body mass, flipper length, bill length and bill depth of the penguins. I omitted 11 NAN values 


Palmer Penguins is a dataset created by Dr. Kristen Gormen.   



***
### **Method overview:** 

**1.  Import libraries**

       
        - Pandas
        - Numpy
        - Matplotlib
        - Seaborn

**2.  Load dataset from url**

**3.  Inspect data**

        - describe the data

**4. Summary Statistics**

**5.  Visualisation of data**
        
        - Barchart
        - Histogram
        - Pairplot
        - Scatterplot
        - Heatmap
        - 
**6. Predictions**

**7. Discussion**

**8. Conclusion**


## Analysis: 
***


### Barcharts:
<p float="left">
        <img src="barchart mean body mass.png" width='400' height='400'>
        <img src="barchart mean flipper length.png" width='400' height='400'>
        <img src="barchart mean bill length.png" width='400' height='400'>
        <img src="barchart mean bill depth.png" width='400' height='400'>
</p>
<br>

### Histograms:

<br>

### Correlation Heatmap:

<br><img src="correlation heatmap.png" width="600" height="500">
<br>
<br>

<br>**Correlation Heatmap per Species:**
<br><img src="correlation heatmap per species.png" width="600" height="500">





### Scatterplot of flipper length vs body mass: <br> 
<br><img src="flipper length vs body mass.png" height="400" width="600">

### Scatterplot of flipper length vs body mass per species:
<p float="left">
<img src="adelie flipper length vs body mass.png" width="400" height="400"> 
<img src="gentoo flipper length vs body mass.png" width="400" height="400">
<img src="chinstrap flipper length vs body mass.png" width="400" height="400">
</p>


### Scatterplot of flipper length vs body mass per species and sex: 
<p float="left">
<img src="adelie flipper length vs body mass per sex.png" width="400" height="400">
<img src="gentoo flipper length vs body mass per sex.png" width="400" height="400">
<img src="chinstrap flipper length vs body mass per sex.png" width="400" height="400">
</p>












