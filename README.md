# Fragment Recruitment Plot for Metagenomic Analysis


Fragment Recruitment Plot displays the graph of aligned metagenomic reads against an organism's reference genome
This plot are useful to display metagenomic reads after performing methods such as digital Normalization(reduction of metagenomic reads). The Percent idenitity and Position are required field to plot a Fragment recruitment Plot.The plot can be created for comparsion of metagenomic reads before and after Normalization.

# R code

R programming can be used to plot Fragment recruitment plot by using ggplot package available in R;

library(ggplot2)

ggplot(Normalization_Acinetobacter_baumannii,aes(POS,Percentage))+ xlab("Genome
Position")+ylab("Percent Identity") + ylim(75,100)+geom_point(color = "Red",size=0.2)
+ggtitle("Fragment Recruitment plot of Acinetobacter_Normalization")


ggplot(Normalization_Deinococcus_radiodurans,aes(POS,Percentage))+ xlab("Genome
Position")+ylab("Percent Identity") + ylim(75,100)+geom_point(color = "Red",size=0.2)
+ggtitle("Fragment Recruitment plot of Deinococcus_Normalization")



