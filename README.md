# -How-to-create-interactive-Animated-plot-in-R-by-using-googleVis-package-
 How to create interactive Animated plot in R by using (googleVis) package 
######  Subscribe this YouTube Channel Data/Fun  ##################
# Package install
install.packages("googleVis")## For Animation plot
install.packages("gapminder")## For Data Set

######  Subscribe this YouTube Channel Data/Fun  ##################
# Recall Package 
library(googleVis)

library(gapminder)

# Data Check
head(gapminder)
?gapminder
######  Subscribe this YouTube Channel Data/Fun  ##################

# Command for Animation plot
ani_plot<-gvisMotionChart(gapminder,
                          xvar = "pop", yvar = "lifeExp",
                          timevar = "year",idvar = "country")

######  Subscribe this YouTube Channel Data/Fun  ##################
# by below command Animated plot will open in web browser 
plot(ani_plot)

######  Subscribe this YouTube Channel Data/Fun  ##################
