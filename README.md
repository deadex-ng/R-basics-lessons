# R-basics-lessons

Session 1
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
