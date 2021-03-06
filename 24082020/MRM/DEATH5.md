 
# DEATH 5 (MRM)
 
## Data: 
- **69 Features**
<details>
<summary>Clinical (15)</summary>
 <pre>
 I.Age, charlson, N.THROMBOZYTEN, N.GOT..AST..HP, N.GPT..ALT..HP, N.LDH.HP, N.CRP.HP, N.FERRITIN.HP, 
 N.PROCALCITONIN, N.INR, N.QUICK..TPZ., N.CREATINKINASE..CK..HP, N.KREATININ..JAFFe..HP, 
 N.UNREIFE.GRANULOZYTEN.ABSOLUT, N.APTT
 </pre>
</details>
<details>
<summary>Proteins (54)</summary>
 <pre>
 A2M, AGT, AHSG, ALB, AMBP, APOA1, APOB, APOE, APOH, B2M, C1QA, C1QB, C1QC, C3, C4A, C4B, C5, CP, 
 CRP, CST3, F10, F11, F12, F13A1, F13B, F2, F5, F9, FGA, FGB, FN1, HBA1, HBB, HP, HPX, KLKB1, LPA, 
 LYZ, ORM1, ORM2, PLG, PPBP, PROS1, RBP4, S100A8, S100A9, SERPINA1, SERPINC1, SERPINF2, SERPING1, 
 SHBG, TF, TTR, VWF
 </pre>
</details>

- **57 Controls, 15 Cases (91 Excluded)**
 <details>
<summary>Group Exclusions</summary>
<br>From the point a patient has a WHO>=5, they die (1) or survive (0)	
<br>
<pre>
| Aux.Id      | Group    | Reason for exclusion                |
|-------------|----------|-------------------------------------|
| C19-CB-0000 | Excluded | Incomplete data                     |
| C19-CB-0001 | Excluded | All points <5                       |
| C19-CB-0003 | Excluded | All points <5                       |
| C19-CB-0005 | Excluded | All points <5                       |
| C19-CB-0008 | 0        |                                     |
| C19-CB-0009 | 0        |                                     |
| C19-CB-0010 | Excluded | All points <5                       |
| C19-CB-0012 | 0        |                                     |
| C19-CB-0013 | 1        |                                     |
| C19-CB-0016 | 1        |                                     |
| C19-CB-0018 | Excluded | All points <5                       |
| C19-CB-0020 | 0        |                                     |
| C19-CB-0021 | 0        |                                     |
| C19-CB-0022 | Excluded | All points <5                       |
| C19-CB-0023 | Excluded | All points <5                       |
| C19-CB-0025 | 0        |                                     |
| C19-CB-0026 | 0        |                                     |
| C19-CB-0029 | Excluded | All points <5                       |
| C19-CB-0030 | Excluded | All points <5                       |
| C19-CB-0032 | 1        |                                     |
| C19-CB-0033 | 0        |                                     |
| C19-CB-0035 | Excluded | All points <5                       |
| C19-CB-0036 | 1        |                                     |
| C19-CB-0037 | Excluded | All points <5                       |
| C19-CB-0038 | Excluded | All points <5                       |
| C19-CB-0039 | 0        |                                     |
| C19-CB-0041 | Excluded | All points <5                       |
| C19-CB-0042 | Excluded | All points <5                       |
| C19-CB-0043 | Excluded | All points <5                       |
| C19-CB-0044 | Excluded | All points <5                       |
| C19-CB-0045 | Excluded | All points <5                       |
| C19-CB-0046 | Excluded | All points <5                       |
| C19-CB-0047 | Excluded | All points <5                       |
| C19-CB-0048 | Excluded | All points <5                       |
| C19-CB-0049 | Excluded | All points <5                       |
| C19-CB-0050 | Excluded | All points <5                       |
| C19-CB-0051 | 0        |                                     |
| C19-CB-0052 | Excluded | All points <5                       |
| C19-CB-0053 | Excluded | All points <5                       |
| C19-CB-0054 | Excluded | All points <5                       |
| C19-CB-0055 | Excluded | All points <5                       |
| C19-CB-0056 | Excluded | All points <5                       |
| C19-CB-0057 | 0        |                                     |
| C19-CB-0058 | 0        |                                     |
| C19-CB-0059 | 1        |                                     |
| C19-CB-0060 | 0        |                                     |
| C19-CB-0061 | 0        |                                     |
| C19-CB-0062 | 0        |                                     |
| C19-CB-0063 | 0        |                                     |
| C19-CB-0064 | 0        |                                     |
| C19-CB-0065 | Excluded | All points <5                       |
| C19-CB-0066 | Excluded | All points <5                       |
| C19-CB-0067 | Excluded | All points <5                       |
| C19-CB-0068 | Excluded | All points <5                       |
| C19-CB-0069 | Excluded | All points <5                       |
| C19-CB-0070 | Excluded | All points <5                       |
| C19-CB-0071 | Excluded | All points <5                       |
| C19-CB-0072 | Excluded | All points <5                       |
| C19-CB-0073 | Excluded | All points <5                       |
| C19-CB-0075 | Excluded | All points <5                       |
| C19-CB-0076 | 0        |                                     |
| C19-CB-0077 | Excluded | All points <5                       |
| C19-CB-0078 | Excluded | All points <5                       |
| C19-CB-0082 | 1        |                                     |
| C19-CB-0083 | 1        |                                     |
| C19-CB-0084 | Excluded | Incomplete data                     |
| C19-CB-0085 | 0        |                                     |
| C19-CB-0086 | Excluded | All points <5                       |
| C19-CB-0087 | Excluded | All points <5                       |
| C19-CB-0088 | Excluded | All points <5                       |
| C19-CB-0089 | Excluded | All points <5                       |
| C19-CB-0090 | 0        |                                     |
| C19-CB-0091 | 0        |                                     |
| C19-CB-0092 | Excluded | All points <5                       |
| C19-CB-0094 | 1        |                                     |
| C19-CB-0095 | 0        |                                     |
| C19-CB-0096 | Excluded | Incomplete data                     |
| C19-CB-0097 | Excluded | All points <5                       |
| C19-CB-0098 | 0        |                                     |
| C19-CB-0099 | 0        |                                     |
| C19-CB-0100 | Excluded | All points <5                       |
| C19-CB-0101 | 1        |                                     |
| C19-CB-0102 | Excluded | Incomplete data                     |
| C19-CB-0103 | 1        |                                     |
| C19-CB-0104 | Excluded | Incomplete data                     |
| C19-CB-0106 | Excluded | Incomplete data                     |
| C19-CB-0107 | Excluded | All points <5                       |
| C19-CB-0108 | 0        |                                     |
| C19-CB-0109 | 0        |                                     |
| C19-CB-0111 | Excluded | Incomplete data                     |
| C19-CB-0112 | 1        |                                     |
| C19-CB-0113 | 0        |                                     |
| C19-CB-0114 | Excluded | All points <5                       |
| C19-CB-0115 | Excluded | All points <5                       |
| C19-CB-0116 | Excluded | All points <5                       |
| C19-CB-0117 | Excluded | All points <5                       |
| C19-CB-0118 | Excluded | All points <5                       |
| C19-CB-0119 | Excluded | All points <5                       |
| C19-CB-0120 | 0        |                                     |
| C19-CB-0121 | Excluded | All points <5                       |
| C19-CB-0122 | 0        |                                     |
| C19-CB-0123 | 0        |                                     |
| C19-CB-0124 | 0        |                                     |
| C19-CB-0125 | Excluded | All points <5                       |
| C19-CB-0126 | 0        |                                     |
| C19-CB-0127 | 0        |                                     |
| C19-CB-0128 | 1        |                                     |
| C19-CB-0129 | 0        |                                     |
| C19-CB-0130 | 0        |                                     |
| C19-CB-0131 | 0        |                                     |
| C19-CB-0132 | Excluded | Refused treatment and died          |
| C19-CB-0133 | 0        |                                     |
| C19-CB-0134 | 0        |                                     |
| C19-CB-0135 | 0        |                                     |
| C19-CB-0136 | 0        |                                     |
| C19-CB-0137 | 0        |                                     |
| C19-CB-0138 | Excluded | Incomplete data                     |
| C19-CB-0139 | Excluded | Incomplete data                     |
| C19-CB-0140 | Excluded | Incomplete data                     |
| C19-CB-0141 | Excluded | Incomplete data                     |
| C19-CB-0142 | 0        |                                     |
| C19-CB-0143 | Excluded | Incomplete data                     |
| C19-CB-0144 | Excluded | Incomplete data                     |
| C19-CB-0145 | Excluded | Incomplete data                     |
| C19-CB-0147 | Excluded | Incomplete data                     |
| C19-CB-0148 | Excluded | Incomplete data                     |
| C19-CB-0149 | Excluded | Incomplete data                     |
| C19-CB-0150 | 0        |                                     |
| C19-CB-0151 | 0        |                                     |
| C19-CB-0152 | 0        |                                     |
| C19-CB-0155 | Excluded | All points <5                       |
| C19-CB-0157 | Excluded | All points <5                       |
| C19-CB-0159 | 0        |                                     |
| C19-CB-0160 | 1        |                                     |
| C19-CB-0162 | 0        |                                     |
| C19-CB-0164 | 0        |                                     |
| C19-CB-0165 | 0        |                                     |
| C19-CB-0166 | Excluded | All points <5                       |
| C19-CB-0167 | Excluded | All points <5                       |
| C19-CB-0168 | Excluded | All points <5                       |
| C19-CB-0169 | 1        |                                     |
| C19-CB-0170 | 1        | But first score missing (assume >5) |
| C19-CB-0175 | Excluded | Incomplete data                     |
| C19-CB-0176 | 0        |                                     |
| C19-CB-0179 | Excluded | All points <5                       |
| C19-CB-0180 | Excluded | Incomplete data                     |
| C19-CB-0181 | 0        |                                     |
| C19-CB-0196 | Excluded | All points <5                       |
| C19-CB-0197 | 0        |                                     |
| C19-CB-0198 | 0        |                                     |
| C19-CB-0199 | 0        |                                     |
| C19-CB-0214 | 0        |                                     |
| C19-CB-0215 | 0        |                                     |
| C19-CB-0216 | Excluded | All points <5                       |
| C19-CB-0217 | Excluded | All points <5                       |
| C19-CB-0218 | 0        |                                     |
| C19-CB-0219 | Excluded | All points <5                       |
| C19-CB-0220 | Excluded | Refused treatment and died          |
| C19-CB-0221 | Excluded | All points <5                       |
| C19-CB-0222 | Excluded | All points <5                       |
| C19-CB-0223 | Excluded | All points <5                       |
| C19-CB-0224 | Excluded | All points <5                       |
| C19-CB-0225 | Excluded | Incomplete data                     |
</pre>
</details>
 
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
## Combined results for 3 different model types (CLINICAL,  PROTEINS, CLINICAL & PROTEINS)
![Image](FINAL_MRM_DIED_5.jpg)

## Top Features
![Image](MRM_DIED_5_TOP.jpg)

## Detailed graphs for each type separately
### Model only on CLINICAL features
![Image](RESULTS_MRM_DIED_5_clinical_1.jpg)
### Model only on PROTEINS features
![Image](RESULTS_MRM_DIED_5_proteins_1.jpg)
### Model on CLINICAL & PROTEINS features
![Image](RESULTS_MRM_DIED_5_full_1.jpg)
