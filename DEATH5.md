# DEATH 5
 
## Data: 
 **201 features (I.Age, charlson, 13 N.(), 186 proteins), 57 Controls, 15 Cases**
 
[Additional information about dataset](/docs/characteristics_Died_5.pdf)
## Example:
![Image](/docs/DIED5_EXAMPLE.jpg)

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
![Image](/docs/DIED5_1.jpg)
## reduce number of proteins
![Image](/docs/DIED5_2.jpg)

![Image](/docs/DIED5_3.jpg)
## Results on 15 selected features
 ```markdown
 svmFit <- train(Group ~ f1 + f2,
                   data = data, method = "svmRadial", preProc = c("center", "scale"),metric = "ROC",
                   trControl = trainControl(method = "cv", classProbs = TRUE, summaryFunction = twoClassSummary))
 ``` 
![Image](/docs/DIED5_4.jpg)
## Networks
![Image](/docs/DIED5_5.jpg)
