# Employee Data Simulation - IT salaries and work experience

Please check the HTML file for full code and graphs!

## Origin of the dataset

The dataset has been found and downloaded on Kaggle - https://www.kaggle.com/datasets/abhayayare/employee-data-simulation-it-industry.
This raw data contains simulated data of 400 employees which ware working on various IT positions.
According to the original poster of the dataset, the dataset was generated using Faker library in Python.

## Explanations of the variables and plan for analysis

This dataset consists of 5 different variables:
1) ID - an unique identifier for each employee (we can ignore it here)

2) gender - either M for Male or F for female

3) experience in years
  
4) position
  
5) salary - in USD

Plan for analysis consists of the following steps:
a. create numerical summaries for each variables

b. check distribution of each variable by graphically showing it with boxplot and histogram/barplot

c. if there will be outliers, make a decision what are we going to do with them?

d. proceed with outlier cleansing

e. try to find relationships between the variables (we can do hypothesis testing, regression analysis, trending...)


Conclusion of the analysis
a. IT employees have scattered distribution of years of experience, and boxplot shows that there are no outliers for that variable

b. Salaries are mostly between 100k and 150k USD, but they have tails on the right/higher side of the distribution - they are only 5 of them, so I decided to delete them, to go further with analysis

c. More male IT employees have between 0-5 years of experience, while more female IT employees have between 8 and 15 years of experience. 

d. When it comes to salary, more male IT employees  have higher salary (between 150-200k USD), and on the female side it is visible that there are some gaps in the middle, but in some paygrades it is visible that females are more paid than males. When it comes to the very peak of salaries, there are more females with that peak of salary than males.

e. When it comes to a relationship between money and years of experience, it is visible that there is a very big span between it. Someone who just starts with their career might have between approximately 140-145k USD, but then later the range of salaries just gets bigger, and being between 50k and 250k USD.

d. if you're interested in salaries per position, and its median value, you can check it here on this picture/graph:


![image](https://github.com/user-attachments/assets/4deafc0f-d493-4ebb-b416-113693012064)

e. Linear regression model attempt between salaries and years of experience: assumptions for a linear model were failed, there was no linearity between, and the tests didn't show proper p-value. As you can see on this picture below, R squared is quite low, and it is probably because this is a simulated data.

![image](https://github.com/user-attachments/assets/523980cf-307e-459d-8b8f-36af9a62d07f)

