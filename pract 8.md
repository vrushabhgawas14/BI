## 8 - Prediction using Logistic Regression

(A dataset called titanic.csv is used.)

```
titanic <- read.table(file = "C:/BI/titanic.csv", sep = ",", header = T, na.strings = (""))
```

```
dim(titanic)
```

```
head(titanic)
```

```
summary(titanic)
```

```
table(titanic$survived)
```

```
titanic$sex<-factor(titanic$sex)
titanic$cabin<-factor(titanic$cabin)
titanic$embarked<-factor(titanic$embarked)
titanic$boat<-factor(titanic$boat)
```

```
is.factor(titanic$sex)
```

```
titanic=titanic[-c(3,8,10,12,13,14)]
```

```
summary(titanic)
```

```
index<-sample(1:nrow(titanic),size=0.6*nrow(titanic))
```

```
train=titanic[index,]
```

```
test=titanic[-index,]
```

```
head(train)
```

```
head(test)
```

```
model <- glm(survived ~.,family=binomial(link=logit),data=train)
```

```
summary(model)
```

```
pred <- predict(model, test, type= "response")
```

```
y_pred <- ifelse(pred > 0.5, 1, 0)
```

```
y_act <- test$survived
```

```
table(y_act,y_pred)
```
