
#yes
library(ggplot2)
library(mosaic)
library(readxl)
library(readr)
library(scales)
library(dplyr)
library(quantomod)
library(readr)
library(ggplot2)
install.packages("tidyverse")
library(tidyverse)
library(readxl)
 Plasma_VL2 <- read_excel("~/Desktop/Rwork/Plasma _VL2.xlsx")
 View(Plasma_VL2) 
 
str(Plasma_VL2)
group1<-data.frame(Plasma_VL2$`Wk post infection`, Plasma_VL2$R2 ,Plasma_VL2$R1,Plasma_VL2$R3,Plasma_VL2$R7,Plasma_VL2$R8)
 group2<-data.frame(Plasma_VL2$`Wk post infection`, Plasma_VL2$R4 ,Plasma_VL2$R5,Plasma_VL2$R6,Plasma_VL2$R9,Plasma_VL2$R10)
 
londgata1<-pivot_longer(group1,col=starts_with("P"),names_to="time",values_to="vl")
londgata2<-pivot_longer(group2,starts_with("P"))
<<<<<<< HEAD
g1<-ggplot(data = group1) + 
     geom_point(mapping = aes(x = group1$Plasma_VL2..Wk.post.infection., y = group1$Plasma_VL2.R2))
g1


=======
>>>>>>> 672c08af1ae81f4d179a0c5262862e0233c707b0

