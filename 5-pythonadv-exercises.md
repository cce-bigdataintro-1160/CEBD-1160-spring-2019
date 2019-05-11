1. We'll be using the titanic `train.csv` file for this exercise, and we'll categorize the gender of the passengers as `0` for male and `1` for female
2. In order to do that create a function called `categorize_gender` that receives a line of the titanic file as a parameter and returns `0` if the passenger is man or `1` if is a woman
```
def categorize_gender(row):
   ???
   return row + [0 or 1]
```

3. Iterate over each row of the file applying your function
4. Add the result of your function call to each row of the dataset, producing a new list
5. Print your new list with an extra field