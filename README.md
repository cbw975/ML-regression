# ML-regression
Uses Linear Regression GD to produce a model for planetary data

## Dataset Info
This is a dataset that consists of various features of NASA confirmed planets. The pertinent ones are:
* Orbital Period [days]
* Orbit Semi-Major Axis [au]
* Stellar Mass [solar mass]

#### Source
Data was produced by the NASA Exoplanet Archive: http://exoplanetarchive.ipac.caltech.edu
* Confirmed planets --> https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=planets
* Downloaded the table as a CSV file --> My file name: planets_2020.09.03_20.35.38.csv
* BUT, for ease of filename usage, I renamed to: planets090320.csv

## Purpose
The purpose in studying this dataset is to classify and compare planetary systems, specifically with regards to their quantitative properties. Plotting and relating these properties can provide insight on the interactions and correlations between them. This can be an important task because of the different properties, compositions, behaviors, etc. of different classes (i.e. by mass or orbital behaviors) of planets. This has effects on their motion, aging, reactions (chemical, atmospheric, etc), interactions with space and bodies around them, etc. Our very understanding of the universe can be based on our studies of the different celestial bodies. 

We train a Linear Regression Gradient Descent model to regress a planet's orbital period based on semi-major axis and solar mass. Linear regression is a linear approach to modelling the relationship between a dependent variable and one or more independent variables. Gradient descent is an iterative optimization algorithm to find the minimum of a function; Here, taht function is the distance or "offness" between the data and the (linear) model.

Our data will include each planet's (features) semi-major axis (a) and solar mass (M), from which the target is orbital period

![period axis relation](https://wikimedia.org/api/rest_v1/media/math/render/svg/5b194cc4755850e6ca14bcc1adc14ecb089b81bf)
