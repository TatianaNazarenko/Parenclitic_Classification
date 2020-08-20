
# DEATH 7 (TRY WITH LOOCV-INTERNAL)

## Model:
 - Internal (for each pair of features f1 and f2): radial SVM (LOOCV) - weights of connection = probability to beloning class 1 
 ```markdown
 
  fitControl <- trainControl(
    method = 'LOOCV',
    number=1,
    savePredictions = 'final',
    classProbs = T,
    seed = as.list(rep(1,(nrow(df_train)+1))),
    summaryFunction = twoClassSummary,
    allowParallel = TRUE
  )
  
  svmFit <- train(Group ~ f1 + f2,
                  data = data,
                  method = "svmRadial",
                  preProc = c("center", "scale"),
                  tuneGrid = expand.grid(sigma = 1, C = 1),
                  metric = "ROC",
                  trControl = fitControl)
 ```
 - External (for network characterisitcs): glm (LOOCV)
 ```markdown
 glmFit <- train(Group ~ (1 network characterisitc),
                   data = data, method = "glm", preProc = c("center", "scale"), metric = "ROC",
                   trControl = trainControl(method = "LOOCV", classProbs = TRUE, summaryFunction = twoClassSummary))
 ```
 
## Results on full set of features
![Image](/docs/temp_DIED7_1.jpg)

## Results on pair of characteristics
![Image](/docs/temp.jpg)

