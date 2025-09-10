# Programming-Assignment-3

PROBLEM 1
For Problem 1, The 2 tasks for was to:
a. Load the corresponding .csv file into a data frame named cars using pandas
b. Display the first five and last five rows of the resulting cars.

My first step was to import pandas as pd and I then imported the "cars.csv" file into the notebook using the code "cars=pd.read_csv('cars.csv)" then printed it using "cars." It showed the list of cars inside the csv file.
After importing and running the files, I then displayed the first and last five rows of the data frame using the codes "cars.head(5)" for the first five rows and "cars.tail(5)" for the last five rows.

Problem 2
Using the same dataframe from Problem 1, the tasks for Problem 2 was to:
a. Display the first five rows with odd-numbered columns (columns 1, 3, 5, 7…) of cars.
b. Display the row that contains the ‘Model’ of ‘Mazda RX4’.
c. How many cylinders (‘cyl’) does the car model ‘Camaro Z28’ have?
d. Determine how many cylinders (‘cyl’) and what gear type (‘gear’) do the car models ‘Mazda RX4 Wag’, ‘Ford Pantera L’ and ‘Honda Civic’ have.

for a. I used the code "cars.iloc[:5, ::2]". ::2 gives the 2nd column starting from index 0
for b. I used the code "cars.loc[cars['Model']== 'Mazda RX4']" which is used to locate the row of the model 'Mazda RX4'.
for c. I used the code "cars.loc[(cars['Model']=='Camaro Z28'),['cyl']]" to locate and display the column 'cyl' of the model 'Camaro Z28'
for d. I used the code "cars.loc[cars["Models"].isin(["Mazda RX4 Wag", "Ford Pantera L", "Honda Civic"]),["cyl", "gear"]}" This is used to locate and display multiple 'Models' and their specific columns.
