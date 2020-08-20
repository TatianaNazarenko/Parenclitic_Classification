# DEATH 7 (with LOOCV in INTERNAL model)

During constructing an edge, each patient gets the _weight_ that is predicted for him by the model built on all other patients, **except him**.

As a result, the entire network of each patient is _pure prediction_.

## Model:
 - Internal (for each pair of features f1 and f2): radial SVM (LOOCV) - weights of connection = probability to beloning class 1 
 ```markdown
 
  fitControl <- trainControl(
    method = 'LOOCV',
    number=1,
    savePredictions = 'final',
    classProbs = T,
    seed = as.list(rep(1,(nrow(data)+1))),
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
Since now the characteristics of different network models are presented here (now each patient has own training-network-model), then every single characteristic of such different networks is now not so good (since all the resulting networks are now different).

![Image](/docs/temp_DIED7_1.jpg)

## Results on pair of characteristics
But the prediction on a couple of them is excellent again (these characteristics compensated for the difference in training models)

![Image](/docs/temp.jpg)

