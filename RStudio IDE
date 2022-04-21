# This is the document for the first coding steps in R


## load and view iris dataset

library (datasets)
data(iris)
View(iris) 

## Now let's find how many different species there are present in the data set.

unique(iris$Species)

## install GGally package

install.packages("GGally", repos = "https://cran.r-project.org", type= "source") 

## loading mtcars dataset

library(datasets)
# Load Data
data(mtcars)
# View first 5 rows
head(mtcars, 5)

#load ggplot package
library(ggplot2)
# create a scatterplot of displacement (disp) and miles per gallon (mpg)
ggplot(aes(x=disp,y=mpg,),data=mtcars)+geom_point()

# Add a title
ggplot(aes(x=disp,y=mpg,),data=mtcars)+geom_point()+ggtitle("displacement vs miles per gallon")

# change axis name
ggplot(aes(x=disp,y=mpg,),data=mtcars)+geom_point()+ggtitle("displacement vs miles per gallon") + labs(x = "Displacement", y = "Miles per Gallon")

#make vs a factor
mtcars$vs <- as.factor(mtcars$vs)
# create boxplot of the distribution for v-shaped and straight Engine
ggplot(aes(x=vs, y=mpg), data = mtcars) + geom_boxplot()


ggplot(aes(x=vs, y=mpg, fill = vs), data = mtcars) + 
  geom_boxplot(alpha=0.3) +
  theme(legend.position="none")
  
  
  ggplot(aes(x=wt),data=mtcars) + geom_histogram(binwidth=0.5)
  
## going back to iris dataset to explore with GGally

library(datasets)
data(iris)

library(GGally)
ggpairs(iris, mapping=ggplot2::aes(colour = Species))



