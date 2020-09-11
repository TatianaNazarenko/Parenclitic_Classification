* [Please find old results (14.08.2020) here](old14082020.md)
* [Please find old results (24.08.2020) here](old24082020.md)
* additional old pages
** temp page](temp.md)
** loocv page](loocv.md)
** loocv 3.09.2020](loocv.md)

# Results 11.09.2020

## IncDNI_Imputation
![Image](/11092020/1.png)
## IncDNI_NoImputation
![Image](/11092020/2.png)
## Final_IncDNI_Imputation
![Image](/11092020/3.png)
## Final_IncDNI_NoImputation
![Image](/11092020/4.png)

### Slight improvement with NNET
 ```markdown
characteristic_model <- function(df_train) {

  df_train$score <- as.factor(df_train$score)
  levels(df_train$score) <- c("first_class","second_class")
  set.seed(123)
  train_control <- trainControl(method = "LOOCV", 
                                number=1,
                                verboseIter = FALSE,
                                classProbs = TRUE, 
                                summaryFunction = twoClassSummary,
                                allowParallel = T,
                                sampling = "rose"
                                )
  
  nnetGrid <-  expand.grid(size = seq(from = 1, to = 10, by = 1),
                           decay = seq(from = 0.1, to = 0.5, by = 0.1))
  
  model <- train(score ~ (.),
                    data = df_train,
                    method = "nnet",
                    tuneGrid = nnetGrid,
                    trControl = train_control,
                    metric = "ROC"
                    ) 
  return(model)
}
 ```
 #### MRM
 ```markdown
 features: c("closeness_mean", "closeness_sd",
             "betweenness_mean", "betweenness_sd",
             "page.rank_mean","page.rank_sd",
             "strength_mean", "strength_sd",
             "authority_score_mean", "authority_score_sd")
 ```
 ![Image](/11092020/4_MRM.png)
  #### FULL SET
 ```markdown
 features: c("closeness_mean", "closeness_sd",
             "page.rank_mean","page.rank_sd",
             "strength_mean", "strength_sd",
             "Eweights_mean", "Eweights_sd")
 ```
  ![Image](/11092020/4_FULL.png)
