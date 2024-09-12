#Lists
list1 <- list(c(1,2,3,4), 34.7, list(0.5,1.0,1.5))

#DataFrame
patients <- data.frame (
  Name = c("John", "Peter", "Paul"),
  Age = c(10, 20, 30)
)

summary(patients)

patients[1]
patients[["Age"]]
patients$age

#Add row
rbind()
new_patients <- rbind(patients, c("Mary", 21))

#Add column
new_col_patients <- cbind(patients, Steps = c(1000, 6000, 2000))

# Remove the first column
Data_Frame_New <- patients[-c(1)]

# Remove the first column
Data_Frame_New <- patients[-c(1)]

#dim
dim(patients)

#number of columns
length(patients)

#Combining DFs
Data_Frame1 <- data.frame (
  Training = c("Strength", "Stamina", "Other"),
  Pulse = c(100, 150, 120),
  Duration = c(60, 30, 45)
)

Data_Frame2 <- data.frame (
  Training = c("Stamina", "Stamina", "Strength"),
  Pulse = c(140, 150, 160),
  Duration = c(30, 30, 20)
)

New_Data_Frame <- rbind(Data_Frame1, Data_Frame2)
New_Data_Frame

#Combining Horizontally using cbind()
Data_Frame3 <- data.frame (
  Training = c("Strength", "Stamina", "Other"),
  Pulse = c(100, 150, 120),
  Duration = c(60, 30, 45)
)

Data_Frame4 <- data.frame (
  Steps = c(3000, 6000, 2000),
  Calories = c(300, 400, 300)
)

New_Data_Frame1 <- cbind(Data_Frame3, Data_Frame4)
New_Data_Frame1

ncol(patients)

