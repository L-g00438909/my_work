<img src="https://mjconroy.com/wp-content/uploads/2023/04/ATU-Logo.png" width="250" height="150">




## Higher Diploma in Science: Computing-Data Analytics 2024
### Module: Principles of Data Analytics


# **Analysis of the Palmer Penguins Dataset**




<img src="https://allisonhorst.github.io/palmerpenguins/reference/figures/lter_penguins.png" alt="penguins" width="500" height='400'/> _Artwork by @Allison_Horst_
***



### Background:

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

<img src="https://upload.wikimedia.org/wikipedia/commons/3/3d/Ant-pen_map_anvers.PNG" width='500' height='500'>
<br>

### Method Overview
#### 1.  Import libraries

       
Pandas
        - Numpy
        - Matplotlib
        - Seaborn

#### 2.  Load dataset from url

#### 3.  Inspect data

describe the data

#### 4. Summary Statistics

#### 5.  Visualisation of data
        
Barchart
        - Histogram
        - Pairplot
        - Scatterplot
        - Heatmap
        - 
#### 6. Predictions

#### 7. Discussion

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

### Pairplot: 
<br><img src="pairplot of numerical variables.png" width='600' height='600'>
<br>



### Scatterplot of flipper length vs body mass: <br> 
<br><img src="flipper length vs body mass.png" height="400" width="600">


There is a strong positive correlation between body mass and flipper length. The correlation coefficient was calculated to be 0.87. 

### Correlation Heatmap:

<br><img src="correlation heatmap.png" width="600" height="500">
<br>
<br>

<br>**Correlation Heatmap per Species:**
<br><img src="correlation heatmap per species.png" width="600" height="500">
### Scatterplot of flipper length vs body mass per species:
<p float="left">
<img src="adelie flipper length vs body mass.png" width="300" height="300"> 
<img src="gentoo flipper length vs body mass.png" width="300" height="300">
<img src="chinstrap flipper length vs body mass.png" width="300" height="300">
</p>


### Scatterplot of flipper length vs body mass per species and sex: 
<p float="left">
<img src="adelie flipper length vs body mass per sex.png" width="300" height="300">
<img src="gentoo flipper length vs body mass per sex.png" width="300" height="300">
<img src="chinstrap flipper length vs body mass per sex.png" width="300" height="300">
</p>












