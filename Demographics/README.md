# Population Demographic Study
## Japan Age Demographics from 1920-2020
A study on the 2020 Census data and historic data to explore the trend in population and age demographics over time.

### Initial Aims
1. Produce visualisations which highlight the importance of the problem and it's consequences.
2. Forecast decades ahead to predict the shift in balance for number of working adults vs children and elderly in the population.
3. Compare with other countries and possibly make predictions for the UK.


### 1) Visualisations show the steadily declining population between 15-64 (working age) and rapidly increasing elderly population

![image](https://user-images.githubusercontent.com/65176466/231733131-24c28e6f-4833-47df-85d5-2a56a3c54aec.png)


![image](https://user-images.githubusercontent.com/65176466/230373933-64bd5569-d784-4d85-9736-1bad5551fc07.png)

### 2)
Holt Exponential Smoothing was used to predict trends of under 15s and over 65s up to 2055. For working age adults this technique didn't produce appropriate results.

15-64s were calculated 15 years into the future, by utilising another dataset. This was the 2020 census data which consisted of a count of the population by single ages. Consequently it was possible to shift these ages up to 15 years into the future, whilst applying a decay coefficient to account for deaths. For 15-64s, simply isolating 95% of the population was the best fit to the trend. I believe this step still has flaws and requires optimisation. For example the 5% decay rate remains the same for 5, 10 and 15 years, whereas this should steadily increase as we predict further into the future

![image](https://user-images.githubusercontent.com/65176466/230374266-e026bc4e-1b7b-4481-b2a8-f6d6a6400898.png)
