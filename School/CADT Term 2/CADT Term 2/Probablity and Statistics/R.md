
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

#  01/04/2025
```R
### 01/04/2025 ###


# "#" to add comment 

2*5      # to show the answer, we press "CTRL+R" 

a=3
b=4
c=a+b 


d=c(4,3,2,1,3,2,2,3,3,4)  # to input data

n=length(d)        # number of element in "Array" or "Vector" d
d[8]             # the eigth element of d

tab0=table(d)        # to create frequency table but in HORIZONTAL format

x=c(1, 2, 3, 4)      # Realisation/Value of X
f=c(1, 3, 4, 2 )      # frequency

tab1=cbind(x,f)      # to create frequency table but in VERTICAL format

f_asc=cumsum(f)      # to create ascending frequency 

tab2=cbind(tab1,f_asc)  # Frequency table with ascending frequency 

# this block is used to create "descending" frequency

f_rev=rev(f)
f_rev_sum=cumsum(f_rev)
f_des=rev(f_rev_sum)

#

tab3=cbind(tab2,f_des)

f_total=sum(f)      # total frequency
f_re=(f/f_total)*100    # relative frequency 

tab4=cbind(tab3,f_re)


f_re_asc=cumsum(f_re)    # ascending relative frequency
f_re_dec=rev(cumsum(rev(f_re)))   #descending relative frequency    


tab_total=cbind(tab4, f_re_asc, f_re_dec)


# to calculate "mean"

d=c(4,3,2,1,3,2,2,3,3,4)  # to input data
n=length(d)
s=sum(d)

xbar=s/n        # find mean by using Definition 

xbar1= mean(d)    # find mean by using built-in function "mean"



##### 08/ 04/ 2025  #######


d=c(4,3,2,1,3,2,2,3,3,4)  
tab0=table(d)  

barplot(tab0)
barplot(tab0, col="blue")
barplot(tab0, col="blue", main="Bar Chart")
?barplot
barplot(tab0, col="blue", main="Bar Chart", xlab="NumberOfAbsence", ylab="Frequency")


pie(tab0)

par(mfrow=c(2,2))  # to show multiple chart in one window  
barplot(tab0)
barplot(tab0, col="red")
barplot(tab0, col="green")
pie(tab0)

?plot

### graphs of some functions 



x=seq(-10,10,0.1)
f=x^2
plot(x,f, type="l", col="red")


g=x^3
plot(x,g, type="l")


par(mfrow=c(1,2))
plot(x,f, type="l", col="red")
plot(x,g, type="l")


plot(f, type="l", ylim=c(-5,5))
lines(g, col="red")
lines(exp(x), col="green")


x=seq(-10,10,0.1)
h=(1/sqrt(2*pi))*exp(-0.5*(x^2))
plot(x,h,type="l", col="red")
```
