# WORSE/BETTER (with AGE)
 [Example of protein pair with Age](https://tatiananazarenko.github.io/Parenclitic_Classification/ex1.html)

## Data: 
 **266 proteins, 12 Controls, 37 Cases**
## Model:
 - Internal (for each pair of proteins p1 and p2): radial SVM (crossvalidation) - weights of connection = probability to beloning class 1
 ```markdown
 svmFit <- train(Group ~ p1 + p2 + AGE,
                   data = data, method = "svmRadial", preProc = c("center", "scale"),metric = "ROC",
                   tuneGrid = expand.grid(sigma = 1, C = 1),
                   trControl = trainControl(method = "cv", number = 5, classProbs = TRUE, summaryFunction = twoClassSummary))
 ```
 - External (for network characterisitcs): glm (LOOCV)
 ```markdown
 glmFit <- train(Group ~ (1 network characterisitc),
                   data = data, method = "glm", preProc = c("center", "scale"), metric = "ROC",
                   trControl = trainControl(method = "LOOCV", classProbs = TRUE, summaryFunction = twoClassSummary))
 ```
 
## Results on full set of proteins
![Image](/docs/WA_1.jpg)
## reduce number of proteins
![Image](/docs/WA_2.jpg)

![Image](/docs/WA_3.jpg)
## Results on 15 selected proteins
![Image](/docs/WA_4.jpg)
## Networks
![Image](/docs/WA_5.jpg)
