# DEATH 6
 
## Data: 
 **200 features (I.Age, charlson, 13 N.(), 185 proteins), 45 Controls, 14 Cases**
## Model:
 - Internal (for each pair of features f1 and f2): radial SVM (crossvalidation) - weights of connection = probability to beloning class 1
 ```markdown
 svmFit <- train(Group ~ f1 + f2,
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
 
## Results on full set of features
![Image](/docs/DIED6_1.jpg)
## reduce number of proteins
![Image](/docs/DIED6_2.jpg)

![Image](/docs/DIED6_3.jpg)
## Results on 15 selected features
 ```markdown
 svmFit <- train(Group ~ f1 + f2,
                   data = data, method = "svmRadial", preProc = c("center", "scale"),metric = "ROC",
                   trControl = trainControl(method = "cv", classProbs = TRUE, summaryFunction = twoClassSummary))
 ```
 
![Image](/docs/DIED6_4.jpg)
## Networks
![Image](/docs/DIED6_5.jpg)
