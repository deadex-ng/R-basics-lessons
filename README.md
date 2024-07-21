# R-basics-lessons

## Session 1

Part 1 
- creating variables
    - numbers and strings
- check what objects are in memory
- basic arithmetic in R
- basic functions in R
    - sqrt()
    - exp()
    - log2()
    - abs()
 - comments

Part 2
- creating vectors
    - x1 <- c(1,3,5,7,9)
- creating sequences in r
    - 2:9
    - seq(from=1, to=7, by=1)
- creating vectors of repeated items
    - rep("male", times=3)
    - rep(1:3, times=5)
    - rep(seq(from=2, to=5, by=0.25), times=5)
- working with one vector
    - x <- 1:5
    -  x + 10
    -  x - 10
    -  x*10
    -  x/2
- working with two vectors
    - x + y
    - x -y
    - x * y
    - x /y
- extracting elements from vectors
    - y[3]
    - y[-3]
    - y[1:3]
    - y[c(1,5)]
    - y[-c(1,5)]
    - y[y<6]
- creating matrix
    - mat <- matrix(c(1,2,3,4,5,6,7,8,9), nrow=3, byrow=TRUE)
    -  mat[1,2]
    -  mat[c(1,3),2]
    -  mat[2,]
    -  mat*10
- Exercise
  - create matrix by column
  - create a matrix from multiple vectors
## Session 2 

Creating Visuals in R 

Bar Plot
- create a data frame 
    - friends <- data.frame(num <-c(2,3,4,5,6), name <-c("Andrew","Ben","Chikondi","Duncan","Evelyn"))
- show the data frame 
    - friends
- load the ggplot package
    - library(ggplot2)
- Install the ggplot package if not installed
    - install.packages("ggplot2")
- Create a bar plot
    - ggplot(data=friends, aes(x=name, y=num)) + geom_bar(stat = "identity")
- Create a horizontal bar plot
    - ggplot(data=friends, aes(x=name, y=num)) + geom_bar(stat = "identity") + coord_flip()

Line Plot

- Create a data frame
    - life_exp <- data.frame(avg_life_expectancy <-c(30,33,45,50,60,73,80,90), year <-c(1985,1990,1995,2000,2005,2010,2015,2020))
- Create a line graph
    - ggplot(data=life_exp, aes(x=year, y=avg_life_expectancy)) + geom_line() + geom_point()

Reources
- [https://ggplot2.tidyverse.org/reference/aes_linetype_size_shape.html](https://ggplot2.tidyverse.org/reference/aes_linetype_size_shape.html)
- [https://moderndive.com/2-viz.html](https://moderndive.com/2-viz.html)

## Read files in R
- read csv file
   - data <- read.csv("C:\\Users\\coco\\Documents\\data.csv")
- read excel files using readxl
   - Install package
      - install.packages("readxl")
   - load the package
      - library("readxl")
   - read excel file
      - books_data <- read_excel("C:\\Users\\coco\\Desktop\\Book1.xlsx")
- read excel files using xlxs
   - Install package
      - install.packages("xlsx")
   - load the package
      - library("xlsx")
   - read excel file
      - data <- read.xlsx("C:\\Users\\coco\\Desktop\\Book1.xlsx", sheetName = "Sheet1")
        


