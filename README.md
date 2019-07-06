# -R-basics
the basics of R language
set.seed(65)

runif(n=9,min=3,max=6)

set.seed(65)

runif(9,3,6)

set.seed(10)

runif(3,10,100)

set.seed(65)

runif(3)
student.df = data.frame( name = c("Sue", "Eva",
                                  "Henry", "Jan"),
                         sex = c("f", "f", "m", "m"), 
                         years = c(21,31,29,19));
student.df


student.df$male.teen = ifelse(student.df$sex == "m" &
                                student.df$years < 20, "T", "F")

student.df

a = 5:8
plot(a)
b = c(5:8)
plot(b)
plot.ts(c(5,3,7,8,3))

x <- c(4,5,6)
x
plot(x)

rn Private Apps Accept Enroll Top10perc Top25perc  [...]
1:     Baylor University     Yes 6075   5349   2367        34        66
2:        Beaver College     Yes 1163    850    348        23        56
3:    Bellarmine College     Yes  807    707    308        39        63
4: Belmont Abbey College     Yes  632    494    129        17        36
5:    Belmont University     Yes 1220    974    481        28        67




dtcollege = data.table(College, keep.rownames = T); class(dtcollege)

?College
head(dtcollege)
summary(dtcollege)

mysubset = dtcollege[40:60]; mysubset

