# Astro497Project
Final Project for Astro 497 at PSU

Project Plan:

Purpose:  
Analyze TTV observations to identify candidates for RV follow-up observations.  

Dataset:  
I plan on using the TTV data provided in [Holczer et al. (2016)](https://iopscience.iop.org/article/10.3847/0067-0049/225/1/9).  
The table of transit times comes from the Kepler mission, and consists of 2,599 Kepler Objects of Interests. This covers the full 17 quarters of the mission. The catalog can be downloaded from a link provided in the paper, but unfortunately it doesn't not seem to download on my computer. This is something that I will have to figure out as a first step. The catalog includes hundreds of thousands of individual transits, so I would imagine that it would be easier to query individual quarters. However, I will need to figure out how to access the catalog first.   

Data wrangling tasks:  
The paper mentions that there are separate tables for duration and depth variations, so I will probably have to utilize joins in order to get the data into one singular table.  

Preliminary models:  
The most basic model to fit TTVs will be linear, so that will be what I will try first. However, as we have learned in class, TTVs require a slightly more advanced model, with an added sinusoidal component. The models will predict which potential exoplanets are good candidates for radial velocity follow up, and which can be ignored. The model will be assessed on the minimum error between the data and the predicted values.  

Potential plots:  
As of now, I am thinking that I will probably show a plot of the actual data points overlayed with the model(s), and then a plot of the error and the parameter values that best minimize the error. The data points will be shown using a scatter plots and linear/curves that fit the data, and the error could be shown using contours. The models could be plotted using time vs transit number, while the error could be a function of loss. Using additional information such as color would definitely be something that I can explore, if I wanted my plots to showcase multiple parameters. It's hard to say exactly what kinds of plots I will have on my final dashboard, that is something that I will decide on once I make multiple plots and see which ones work the best.    

Preliminary schedule:  
Since I plan on working alone, the schedule is flexible. However, I do plan on putting in ~3 hours each week on this project. If I feel like I am lagging behind, then I will put in more hours accordingly. 
