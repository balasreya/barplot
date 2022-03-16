# barplot
name<-c("sreya","saswi","swathi","varsha","pragna")
gender<-c("male","female","thada","dingding","female")
no<-c("76","74","43","76","09")
print("enter the total ")
total<-scan()
dataframe<-data.frame("s.no","name","gender","no","total")
write.csv("dataframe","rvr&jc.csv",row.name=F)
x<-read.csv("rvr&jc.csv")
view(x)
barplot(x$total,
        xlab="toal students",
        ylab="average students",
        main="rvr&jc",
        names.avg=x$name,
        col=rainbow(length(name)),
        las=2)
