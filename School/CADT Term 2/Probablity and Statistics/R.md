
Take only pictures, leave only footprints.

R swirl course at lesson 5

done with matrices and dataframes

```R
year %% 4 == 0 & (year %% 100 != 0 | year %% 400 == 0)
```


# Frequency counter

```R
x <- c(1,2,6,7,3,4,1,2,1,2,2)

table(x)

as.data.frame(table(x))

rle(sort(x))

tabulate(x)

aggregate(x, list(num=x), length)

```


Analysis
```R
x <- c() #vector of our data
df <- as.data.frame(table(x)) #dataframe of vector
n <- sum(df[[2]])

#Culmulative frequency
cf <- vector("list", length(df[[2]]))
index <- 1
for(x in df[[2]]){
	if(index == 1){
        cf[[index]] <- x
	} else {
        cf[[index]] <- cf[[index-1]] + x
	}
    index <- index+1
}
#Inverse Culmulative frequency
icf <- vector("list", length(df[[2]]))
index <- 1
for(x in df[[2]]){
    if(index == 1){
        icf[[index]] <- n
    } else {
        icf[[index]] <- icf[[index-1]] - x
    }
    index <- index+1
}



```

```R
data_set <- c(1,2,6,7,3,4,1,2,1,2,2)
df <- as.data.frame(table(data_set)) #dataframe of vector
n <- sum(df[[2]])

index <- 1
cf <- vector("list", length(df[[2]]))
for(x in df[[2]]){
	if(index == 1){
        cf[[index]] <- x
	} else {
        cf[[index]] <- cf[[index-1]] + x
	}
    index <- index+1
}

index <- 1
rcf <- vector("list", length(df[[2]]))
for(x in cf){
    rcf[index] <- cf[[index]]/n
    index <- index+1
}

index <- 1
icf <- vector("list", length(df[[2]]))
index <- 1
for(x in df[[2]]){
    if(index == 1){
        icf[[index]] <- n
    } else {
        icf[[index]] <- icf[[index-1]] - x
    }
    index <- index+1
}


index <- 1
ricf <- vector("list", length(df[[2]]))
for(x in icf){
    ricf[index] <- icf[[index]]*100/n
    index <- index+1
}

mean <- mean(data_set)
mode <- names(sort(-table(data_set)))[1] #sort table
median <- median(data_set)



```