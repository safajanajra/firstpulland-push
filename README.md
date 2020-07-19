
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
 
 