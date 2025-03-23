### Title : Construct a Decision Tree in R

<!-- 1 -->

```
install.packages("party")
```

<!-- 2 -->

```
library(party)
```

<!-- 3 -->

```
print(readingSkills)
```

<!-- 4 -->

```
input <- readingSkills[c(1:105),]
print(input)
```

<!-- 5 -->

```
output <- ctree(nativeSpeaker ~ age + shoeSize + score, input)
print(output)
```

<!-- 6 -->

```
plot(output)
```
