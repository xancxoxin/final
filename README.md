이름 : 강승희
학번 : 602377101
동작여부 : 동작하지 않음
install.packages("animation")
setwd("D:/602377101_ksh")
library(animation)
animation::ani.options(interval = 1)
runif(5, min=0, max=100)
nb <-c('97.35211', '22.66414' ,'53.62073', '54.07392', '96.44881')
nbt <- table(nb)
barplot(nbt, main='춤추는 막대 그래프',
        ylim=c(0, 100),
        col=c('blue', 'yellow','red','green','orange'))
ani.pause()