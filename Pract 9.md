## 9 - Time Series analysis in R

- **(Yearly Data : Frequency = 1)**
- **(Monthly Data : Frequency = 12)**
- **(Quaterly Data : Frequency = 4)**

```
rainfall <- c(799,1174.8,865.1,1334.6,635.4,918.5,685.5,998.6,784.2,985,882.8,1071)
```

```
rainfall.timeseries <- ts(rainfall,start =2002,end=2012,frequency = 1)
```

```
print(rainfall.timeseries)
```

```
png(file = "rainfall.png")
```

```
plot(rainfall.timeseries)
```

```
dev.off()
```

```
plot(rainfall.timeseries)
```

#### For Monthly and Quaterly repeat the exact same steps but change the frequencies
