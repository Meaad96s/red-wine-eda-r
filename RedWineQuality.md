Red Wine Quality Exploratory Anlysis by Meaad AlRshoud
========================================================
# Load all of the packages




```
## [1] "Dataset Attributes"
```

```
## 
## * X 
## * fixed.acidity 
## * volatile.acidity 
## * citric.acid 
## * residual.sugar 
## * chlorides 
## * free.sulfur.dioxide 
## * total.sulfur.dioxide 
## * density 
## * pH 
## * sulphates 
## * alcohol 
## * quality 
## 
## <!-- end of list -->
```

# Univariate Plots Section



```
## 
## -------------------------------------------------------------------
##        X          fixed.acidity   volatile.acidity    citric.acid  
## ---------------- --------------- ------------------ ---------------
##   Min.  : 1.0     Min.  : 4.60     Min.  :0.1200     Min.  :0.000  
## 
##  1st Qu.: 400.5   1st Qu.: 7.10    1st Qu.:0.3900    1st Qu.:0.090 
## 
##  Median : 800.0   Median : 7.90    Median :0.5200    Median :0.260 
## 
##   Mean : 800.0     Mean : 8.32      Mean :0.5278      Mean :0.271  
## 
##  3rd Qu.:1199.5   3rd Qu.: 9.20    3rd Qu.:0.6400    3rd Qu.:0.420 
## 
##  Max.  :1599.0    Max.  :15.90     Max.  :1.5800     Max.  :1.000  
## -------------------------------------------------------------------
## 
## Table: Red Wine Quality summary (continued below)
## 
##  
## -------------------------------------------------------------------------------
##  residual.sugar      chlorides      free.sulfur.dioxide   total.sulfur.dioxide 
## ---------------- ----------------- --------------------- ----------------------
##  Min.  : 0.900    Min.  :0.01200       Min.  : 1.00           Min.  : 6.00     
## 
##  1st Qu.: 1.900   1st Qu.:0.07000      1st Qu.: 7.00         1st Qu.: 22.00    
## 
##  Median : 2.200   Median :0.07900      Median :14.00         Median : 38.00    
## 
##   Mean : 2.539     Mean :0.08747        Mean :15.87           Mean : 46.47     
## 
##  3rd Qu.: 2.600   3rd Qu.:0.09000      3rd Qu.:21.00         3rd Qu.: 62.00    
## 
##  Max.  :15.500    Max.  :0.61100       Max.  :72.00          Max.  :289.00     
## -------------------------------------------------------------------------------
## 
## Table: Table continues below
## 
##  
## ---------------------------------------------------------------------------------
##     density            pH           sulphates         alcohol         quality    
## ---------------- --------------- ---------------- --------------- ---------------
##  Min.  :0.9901    Min.  :2.740    Min.  :0.3300    Min.  : 8.40    Min.  :3.000  
## 
##  1st Qu.:0.9956   1st Qu.:3.210   1st Qu.:0.5500   1st Qu.: 9.50   1st Qu.:5.000 
## 
##  Median :0.9968   Median :3.310   Median :0.6200   Median :10.20   Median :6.000 
## 
##   Mean :0.9967     Mean :3.311     Mean :0.6581     Mean :10.42     Mean :5.636  
## 
##  3rd Qu.:0.9978   3rd Qu.:3.400   3rd Qu.:0.7300   3rd Qu.:11.10   3rd Qu.:6.000 
## 
##  Max.  :1.0037    Max.  :4.010    Max.  :2.0000    Max.  :14.90    Max.  :8.000  
## ---------------------------------------------------------------------------------
```

# Univariate Analysis

# Explore Data set attribute to get insight

![plot of chunk Quality_Distribution](figure/Quality_Distribution-1.png)
 Most wine quiality falls under 5-6 score. Kind of normal distribution since it's 
(low-high-low) The distribution has no outliers.

![plot of chunk fixed.acidity](figure/fixed.acidity-1.png)

The plot of fixed acidity is positively skewed, about 60 wine has around 8-10 
Aacidity and there is outliers. Thats why the mean (8.32) is larger than median (7.9)

![plot of chunk volatile.acidity](figure/volatile.acidity-1.png)
The mean of Volatile Acidity is 0.52 & median is also 0.52 but it's not normal 
distribution it's bimodal as the bar plot shows. There is outliers.


![plot of chunk citric.acid](figure/citric.acid-1.png)
Critic Acid has a mean of 0.27 and median of 0.26 the distribution is low 
with two individual peaks and one outlier of high critic acidity
This might indicate a poor data gathering or governance of the sensors.


  
  ![plot of chunk residual.sugar](figure/residual.sugar-1.png)
Residual Sugar has a mean of 2.54 and median of 2.2. 
Which justify the positively skewed graph at 2; outliers of high resifual sugar exists.


![plot of chunk chlorides](figure/chlorides-1.png)
 Chlorides has a mean of 0.9 and median of 0.8 It's also positively skewed at 0.1
 Chlorides has outliers.


![plot of chunk free.sulfur.dioxide](figure/free.sulfur.dioxide-1.png)
Free Sulfur Dioxide has a mean of 15.87 and median of 14
Right skewed and most wines tops free sulfur dioxide at 7 , outliers exists


![plot of chunk total.sulfur.dioxide](figure/total.sulfur.dioxide-1.png)
Total Sulfur Dioxide has a mean of 46 and median of 38. As this attribute and the previous 
one present the same chemical propery they share thame distribution

![plot of chunk density](figure/density-1.png)
Density has a mean of 0.99 and median of 0.99
from mean & median and the plot we are firm it's normal distribution

![plot of chunk pH](figure/pH-1.png)
pH has a mean of 3.31 and median of 3.31
from mean & median and the plot we are firm it's normal distribution

![plot of chunk sulphates](figure/sulphates-1.png)
Sulphates has a mean of 0.65 and median of 0.62
positively skewed between 0.5-0.75 and has outliers.


![plot of chunk alcohol](figure/alcohol-1.png)
Alcohol has a mean of 10.42 and median of 10.20
Right skewed and most wines tops free sulfur dioxide at 7 , outliers exists




### What is the structure of your dataset?

print("Red wine Quality data set has 1,599 rows and 11 attributes along with the target attribute it's 12")
print(" The target attribute is quality and the only categoral attribute in the data set")
print(" The remaining attributes represent numerical chemical properties of the wine")


### What is/are the main feature(s) of interest in your dataset?

Print("my main interest is what features contributes more to the quality of wine")

### What other features in the dataset do you think will help support your
##investigation into your feature(s) of interest?

print("Most attributes have same distribution either right, normal or bimodal, I think all of them affects the quality")
  
  ### Of the features you investigated, were there any unusual distributions? 
print("Critic Acid")

 ### Did you perform any operations on the data to tidy, adjust, or change the form \
###of the data? If so, why did you do this?


# Bivariate Plots Section

#

```
## 'data.frame':	1599 obs. of  13 variables:
##  $ X                   : int  1 2 3 4 5 6 7 8 9 10 ...
##  $ fixed.acidity       : num  7.4 7.8 7.8 11.2 7.4 7.4 7.9 7.3 7.8 7.5 ...
##  $ volatile.acidity    : num  0.7 0.88 0.76 0.28 0.7 0.66 0.6 0.65 0.58 0.5 ...
##  $ citric.acid         : num  0 0 0.04 0.56 0 0 0.06 0 0.02 0.36 ...
##  $ residual.sugar      : num  1.9 2.6 2.3 1.9 1.9 1.8 1.6 1.2 2 6.1 ...
##  $ chlorides           : num  0.076 0.098 0.092 0.075 0.076 0.075 0.069 0.065 0.073 0.071 ...
##  $ free.sulfur.dioxide : num  11 25 15 17 11 13 15 15 9 17 ...
##  $ total.sulfur.dioxide: num  34 67 54 60 34 40 59 21 18 102 ...
##  $ density             : num  0.998 0.997 0.997 0.998 0.998 ...
##  $ pH                  : num  3.51 3.2 3.26 3.16 3.51 3.51 3.3 3.39 3.36 3.35 ...
##  $ sulphates           : num  0.56 0.68 0.65 0.58 0.56 0.56 0.46 0.47 0.57 0.8 ...
##  $ alcohol             : num  9.4 9.8 9.8 9.8 9.4 9.4 9.4 10 9.5 10.5 ...
##  $ quality             : int  5 5 5 6 5 5 5 7 7 5 ...
```

![plot of chunk Correlation](figure/Correlation-1.png)![plot of chunk Correlation](figure/Correlation-2.png)

```
## 
## -------------------------------------------------------------------------
##           &nbsp;                X       fixed.acidity   volatile.acidity 
## -------------------------- ----------- --------------- ------------------
##           **X**                 1          -0.2685         -0.008815     
## 
##     **fixed.acidity**        -0.2685          1             -0.2561      
## 
##    **volatile.acidity**     -0.008815      -0.2561             1         
## 
##      **citric.acid**         -0.1536       0.6717           -0.5525      
## 
##     **residual.sugar**      -0.03126       0.1148           0.001918     
## 
##       **chlorides**          -0.1199       0.09371           0.0613      
## 
##  **free.sulfur.dioxide**     0.09048       -0.1538          -0.0105      
## 
##  **total.sulfur.dioxide**    -0.1178       -0.1132          0.07647      
## 
##        **density**           -0.3684        0.668           0.02203      
## 
##           **pH**              0.136        -0.683            0.2349      
## 
##       **sulphates**          -0.1253        0.183            -0.261      
## 
##        **alcohol**           0.2451       -0.06167          -0.2023      
## 
##        **quality**           0.06645       0.1241           -0.3906      
## -------------------------------------------------------------------------
## 
## Table: Table continues below
## 
##  
## ---------------------------------------------------------------------
##           &nbsp;            citric.acid   residual.sugar   chlorides 
## -------------------------- ------------- ---------------- -----------
##           **X**               -0.1536        -0.03126       -0.1199  
## 
##     **fixed.acidity**         0.6717          0.1148        0.09371  
## 
##    **volatile.acidity**       -0.5525        0.001918       0.0613   
## 
##      **citric.acid**             1            0.1436        0.2038   
## 
##     **residual.sugar**        0.1436            1           0.05561  
## 
##       **chlorides**           0.2038         0.05561           1     
## 
##  **free.sulfur.dioxide**     -0.06098         0.187        0.005562  
## 
##  **total.sulfur.dioxide**     0.03553         0.203         0.0474   
## 
##        **density**            0.3649          0.3553        0.2006   
## 
##           **pH**              -0.5419        -0.08565       -0.265   
## 
##       **sulphates**           0.3128         0.005527       0.3713   
## 
##        **alcohol**            0.1099         0.04208        -0.2211  
## 
##        **quality**            0.2264         0.01373        -0.1289  
## ---------------------------------------------------------------------
## 
## Table: Table continues below
## 
##  
## -----------------------------------------------------------------------
##           &nbsp;            free.sulfur.dioxide   total.sulfur.dioxide 
## -------------------------- --------------------- ----------------------
##           **X**                   0.09048               -0.1178        
## 
##     **fixed.acidity**             -0.1538               -0.1132        
## 
##    **volatile.acidity**           -0.0105               0.07647        
## 
##      **citric.acid**             -0.06098               0.03553        
## 
##     **residual.sugar**             0.187                 0.203         
## 
##       **chlorides**              0.005562                0.0474        
## 
##  **free.sulfur.dioxide**             1                   0.6677        
## 
##  **total.sulfur.dioxide**         0.6677                   1           
## 
##        **density**               -0.02195               0.07127        
## 
##           **pH**                  0.07038               -0.06649       
## 
##       **sulphates**               0.05166               0.04295        
## 
##        **alcohol**               -0.06941               -0.2057        
## 
##        **quality**               -0.05066               -0.1851        
## -----------------------------------------------------------------------
## 
## Table: Table continues below
## 
##  
## ----------------------------------------------------------------------------------
##           &nbsp;            density       pH      sulphates   alcohol    quality  
## -------------------------- ---------- ---------- ----------- ---------- ----------
##           **X**             -0.3684     0.136      -0.1253     0.2451    0.06645  
## 
##     **fixed.acidity**        0.668      -0.683      0.183     -0.06167    0.1241  
## 
##    **volatile.acidity**     0.02203     0.2349     -0.261     -0.2023    -0.3906  
## 
##      **citric.acid**         0.3649    -0.5419     0.3128      0.1099     0.2264  
## 
##     **residual.sugar**       0.3553    -0.08565   0.005527    0.04208    0.01373  
## 
##       **chlorides**          0.2006     -0.265     0.3713     -0.2211    -0.1289  
## 
##  **free.sulfur.dioxide**    -0.02195   0.07038     0.05166    -0.06941   -0.05066 
## 
##  **total.sulfur.dioxide**   0.07127    -0.06649    0.04295    -0.2057    -0.1851  
## 
##        **density**             1       -0.3417     0.1485     -0.4962    -0.1749  
## 
##           **pH**            -0.3417       1        -0.1966     0.2056    -0.05773 
## 
##       **sulphates**          0.1485    -0.1966        1       0.09359     0.2514  
## 
##        **alcohol**          -0.4962     0.2056     0.09359       1        0.4762  
## 
##        **quality**          -0.1749    -0.05773    0.2514      0.4762       1     
## ----------------------------------------------------------------------------------
```
# From the correlation matrix, 
# Positive correlation between (alcohol & Quality)=0.476
# Negative Correlation (Volatile Acidity & Quality)=-0.39

![plot of chunk Heatmap](figure/Heatmap-1.png)
# The heatmap support the previos findings


```
## The following objects are masked from red_wine (pos = 3):
## 
##     alcohol, chlorides, citric.acid, density, fixed.acidity,
##     free.sulfur.dioxide, pH, quality, residual.sugar, sulphates,
##     total.sulfur.dioxide, volatile.acidity, X
```

![plot of chunk Bivariate_Plots](figure/Bivariate_Plots-1.png)![plot of chunk Bivariate_Plots](figure/Bivariate_Plots-2.png)![plot of chunk Bivariate_Plots](figure/Bivariate_Plots-3.png)


# Bivariate Analysis

### Talk about some of the relationships you observed in this part of the \
The high correlation between Quality and alcohol which is reasonable 0.47
From the scatter plot we see the alcohol line is rising along.
The low correlation between quality and volatile acidity -0.39

### Did you observe any interesting relationships between the other features \
From the correlation matrix I observed prominent high correlation between chemical properties
I will list the positive and negative 
Positive cor: The density of water increase wine quality by balancing the other properties.
Negative cor:(pH & Fixed acidity)=-0.68: the more acidity the pH level , 
(pH & Critic Acidity)= -0.54: the more acidity the pH level,
(density & alcohol)=-0.49: As the desnity of water increases the alcohol dissolve and decreases.

, (Volatile Acidity & critic acidity)=-0.55: They are both acids types that intersection wach other.

### What was the strongest relationship you found?
1- Density and fixed acidity =0.668
2- critic acid and fixed acidity =0.67

# Multivariate Plots Section


![plot of chunk Multivariate_Plots](figure/Multivariate_Plots-1.png)

```
## Error in +ggtitle("Multivariant plot"): invalid argument to unary operator
```
The plot consists of target with strong and negative correlated features.
The alcohol is immersed in the midde, the overall color of distance is pink which means low volatile acidity
# Multivariate Analysis

```
## 
## Call:
## lm(formula = as.numeric(quality) ~ alcohol + volatile.acidity + 
##     sulphates + citric.acid + fixed.acidity + pH, data = training_data)
## 
## Residuals:
##      Min       1Q   Median       3Q      Max 
## -2.69045 -0.38863 -0.06562  0.45943  1.97867 
## 
## Coefficients:
##                  Estimate Std. Error t value Pr(>|t|)    
## (Intercept)       3.47843    0.64885   5.361 9.83e-08 ***
## alcohol           0.32123    0.01824  17.609  < 2e-16 ***
## volatile.acidity -1.34525    0.12543 -10.725  < 2e-16 ***
## sulphates         0.68824    0.11484   5.993 2.68e-09 ***
## citric.acid      -0.58474    0.15391  -3.799 0.000152 ***
## fixed.acidity     0.03619    0.01667   2.171 0.030122 *  
## pH               -0.32511    0.17224  -1.888 0.059310 .  
## ---
## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
## 
## Residual standard error: 0.658 on 1272 degrees of freedom
## Multiple R-squared:  0.3385,	Adjusted R-squared:  0.3354 
## F-statistic: 108.5 on 6 and 1272 DF,  p-value: < 2.2e-16
```


### Talk about some of the relationships you observed in this part of the \
For the quality relationships with other features:
* Alcohol and Sulaphate amount affects wine positively.
* Citric Acid, has minor affect of improving the wine quality.

### Were there any interesting or surprising interactions between features?
The three acidity features, Volatile acidity, critic acidity and fixed acidity. 
Fixed acidity and volatile acidity has negative correlation.
but Fixed acidity and critic acid has positive correlation.

### OPTIONAL: Did you create any models with your dataset? 
The model is built with 6 attributes of strong or negative correlation.
The model summary: quality = 2.985 + 0.276xalcohol - 2.985xvolatile.acidity + 0.908xsulphates + 0.065xcitric.acid - -1.763*chlorides - 0.002xtotal.sulfur.dioxide 
There was not enough information decide confidence level. Value of R squared value are low, alcohol contributes to 22% of the Wine Quality.
The lack of many information may be due of containing 'Average' quality wines in the dataset.


# Final Plots and Summary


### Plot One
![plot of chunk Plot_One](figure/Plot_One-1.png)

### Description One
Positive Correlation:
  
  1. Density with Fixed Acidity. Which is reasonable
2. Quality and Alcohol. which is also reasonable
3. Fixed acidity and critic acid.

Negative:
  1. The strongest correlation in the plot is between Volatile acidity and pH.
Though, they should be negative since pH is a base that sould lower the acidity.
2. Alcohol with density. Mathmatically as water increases alcohol dissolves.
3. Fixed acidity and volatile acidity

### Plot Two
![plot of chunk Plot_Two](figure/Plot_Two-1.png)

### Description Two

Large spread of data of each concentration level 


### Plot Three
![plot of chunk Plot_Three](figure/Plot_Three-1.png)

```
## Error in +ggtitle("Multivariant plot"): invalid argument to unary operator
```

### Description Three
Quality of wine mostly between 5-7 with alcohol amount of 9 to 13 While in both condition
the volatile acidity is mainly 0.4
------
  
  # Reflection
The major contribution to quality of the features is alcohol, which is predictable and the analysis is right.
Also, Sulfates has a small positive contribution. Its normally used to prevent rotting.
A down side contribution to quality is Volatile acidity , Volatile acidity affects to the acidic taste.
I struggled with lack of data to statistics.
also with data accuracy and data collection. Some were not reasonable.
Most correlation went as expected and the overall analysis is expected.
What surprised how pH and volatile acidity are positively correlated.
The data could use a better data collection and raw data without average modificaton.
A linear model is build upon  6 features.

  
