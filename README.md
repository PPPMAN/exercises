#Code for Section 3.7, exercise 3.1, from Zuur,Ieno and Meesters (2009) 

BirdFlu=read.csv("BirdFlu.csv",header=TRUE,dec=".")

names(BirdFlu)
#a "X" appears before the variable name. Why?

str(BirdFlu)

#What is the total number of bird flu cases in 2003 and in 2005?
Sum.2003=sum(BirdFlu$X2003.cases)
print(Sum.2003)

Sum.2005=sum(BirdFlu$X2005.cases)
print(Sum.2005)

#Which country has had the most cases?
BirdFlu$TotalCases=BirdFlu$X2003cases + BirdFlu$X2004cases + BirdFlu$X2005cases + BirdFlu$X2006cases + BirdFlu$X2007cases + BirdFlu$X2008cases
BirdFlu


#Which country has had the least bird flu deaths?
BirdFlu$TotalDeaths=BirdFlu$X2003deaths + BirdFlu$X2004deaths + BirdFlu$X2005deaths + BirdFlu$X2006deaths + BirdFlu$X2007deaths + BirdFlu$X2008deaths
BirdFlu

#What is the total number of cases per year?
Sum.2003=sum(BirdFlu$X2003.cases)
print(Sum.2003)
Sum.2004=sum(BirdFlu$X2004.cases)
print(Sum.2004)
Sum.2005=sum(BirdFlu$X2005.cases)
print(Sum.2005)
Sum.2006=sum(BirdFlu$X2006.cases)
print(Sum.2006)
Sum.2007=sum(BirdFlu$X2007.cases)
print(Sum.2007)
Sum.2008=sum(BirdFlu$X2008.cases)
print(Sum.2008)

##################################################################################################

