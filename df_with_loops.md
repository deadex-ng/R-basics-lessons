# Create a simple data frame
```r
df <- data.frame(
  Name = c("John", "Alice", "Bob", "Emily"),
  Age = c(28, 34, 22, 45),
  Salary = c(50000, 60000, 45000, 70000)
)
```

# Display the original data frame

```r
print("Original Data Frame:")
print(df)
``

# Add a calculated column 'Bonus' using a for loop

df$Bonus <- NA  # Initialize the new column with NA
```

# Calculate bonus as 10% of the salary for each person using a for loop

```r
for (i in 1:nrow(df)) {
  df$Bonus[i] <- df$Salary[i] * 0.10
}
```

# Display the updated data frame
```r
print("Data Frame with Bonus Column:")
print(df)
```

# While Loop
```r
# variable to store current number
number = 1

# variable to store current sum
sum = 0

# while loop to calculate sum
while(number <= 10) {

  # calculate sum
  sum = sum + number
    
  # increment number by 1
  number = number + 1
}

print(sum)
```
