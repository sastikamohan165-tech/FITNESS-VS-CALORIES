# FITNESS-VS-CALORIES


Skip to content
Using Gmail with screen readers
Enable desktop notifications for Gmail.
   OK  No thanks
1 of 304
(no subject)
Inbox

Devaki K
2:09 PM (0 minutes ago)
to me

fitness <- data.frame(
  Day = 1:12,
  Steps = c(3000,3500,4000,5000,6000,7000,8000,8500,9000,9500,10000,11000),
  Calories = c(150,170,190,230,260,300,340,360,380,400,430,470)
)
print(fitness)
x<-(3000,3500,4000,5000,6000,7000,8000,8500,9000,9500,10000,11000)
y<-(150,170,190,230,260,300,340,360,380,400,430,470)

plot(fitness$Steps, fitness$Calories,
     main = "Steps vs Calories",
     xlab = "Steps",
     ylab = "Calories Burned",
     col = "blue",
     pch = 19)

plot(fitness$Day, fitness$Steps,
     type = "l",
     main = "Steps Over Days",
     xlab = "Day",
     ylab = "Steps",
     col = "green",
     lwd = 2)

barplot(fitness$Calories,
        names.arg = fitness$Day,
        main = "Calories Burned Each Day",
        xlab = "Day",
        ylab = "Calories",
        col = "orange")


max_steps <- max(fitness$Steps)
day_max_steps <- fitness$Day[which.max(fitness$Steps)]

cat("Maximum Steps:", max_steps, "\n")
cat("Day with Maximum Steps:", day_max_steps, "\n")
