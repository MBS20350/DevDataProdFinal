DDP Final Project
========================================================
author: Mark Sucato
date: 01 Oct 2021
autosize: true

"Predict Adult Children's Height" Shiny App
========================================================
- Predicts adult childrens' heights using birth gender and parent's heights
- Outputs include predicted height and a prediction interval using
user-specified confidence level
- Applet also features a gender-specific 3D multivariate scatterplot with
regression plane
- Applet location:  https://marksucato.shinyapps.io/DDPfinalproject/

Applet Screenshot
========================================================
![alt text](App2.png)


Background and Instructions
========================================================
Background
-  Galton's 1886 article "Regression Towards Mediocrity in Hereditary
Stature" analyzed the heights of 928 adult children and their pairs of parents to illustrate his linear regression model
- Applet uses several variables from original dataset to predict adult childrens' heights

***
Instructions
- Input the parents' heights in inches, child's birth gender and desired
confidence level
- Click 'Calculate'
- 3D scatterplot can be manipulated via user input

Multiple Regression Model Coefficients
========================================================

```
lm(formula = height ~ mother + father + gender, data = data)
```

```
(Intercept)      mother      father     genderM 
 15.3447600   0.3214951   0.4059780   5.2259513 
```


