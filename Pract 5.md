## 5 - Prediction using Linear Regression

```
Height <- c(151, 174, 138, 186, 128, 136, 179, 163, 152, 131)
```

```
Weight <- c(63, 81, 56, 91, 47, 57, 76, 72, 62, 48)
```

```
relation <- lm(Weight~Height)
```

```
print(relation)
```

```
print(summary(relation))
```

```
a <- data.frame(Height=170)
```

```
result <- predict(relation,a)
```

```
print(result)
```

```
a <- data.frame(Height=190)
```

```
result <- predict(relation,a)
```

```
print(result)
```

```
plot(Height,Weight)
```

```
plot(Height,Weight,pch=15, cex=1.3, col="blue" ,main="Height and
Weight Regression", xlab="Height(cm)", ylab="Weight(kg)")
```

```
abline(lm(Weight~Height))
```
