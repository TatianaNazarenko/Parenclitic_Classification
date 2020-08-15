 
# WORSE/BETTER (original)
 
## Data: 
- **200 Features**
<details>
<summary>Clinical (13)</summary>
 <pre>
I.Age, charlson, N.THROMBOZYTEN, N.GOT..AST..HP, N.GPT..ALT..HP, N.LDH.HP, N.CRP.HP, N.PROCALCITONIN, 
N.INR, N.QUICK..TPZ., N.CREATINKINASE..CK..HP, N.KREATININ..JAFFe..HP, N.APTT
 </pre>
</details>
<details>
<summary>Proteins (187)</summary>
 <pre>
C4A.C4B, ALB, TTR, MST1, MASP1, ITIH1, IGLC7, A2M, C7, APOB, KNG1, APOE, C3, FN1, CFI, F10, PIGR, SERPINC1, 
IGLC7.IGLL5, HRG, SERPINA3, TF, IGLC2.IGLC3, IGKC, ITIH4, C8G, ITIH2, IGHV3.23, IGHV3.64D, CP, SELL, C4B, 
C9, AFM, CST3, C5, AMBP, CD14, VWF, A2M.PZP, GSN, FCGBP, IGHV3.13, CFH, AZGP1, ACTA2.ACTB.ACTG1.ACTG2, CPN2, 
PGLYRP2, IGLL5, APOA1, FGB, CFB, FGG, FBLN1, C6, APOA4, C8A, CNDP1, LRG1, CRP, C4BPB, S100A8, IGHG1.IGHG3, 
AGT, F11, CD44, FGA, SERPINF1, APOL1, SERPINA7, APOH, IGHV5.51, PROS1, IGHV1.18, IGKV1.5, IGKV3.20, CLU, LBP, 
CFD, PLG, LPA, A1BG, HP, HP.HPR, SERPINA1, C2, SERPINA6, F5, IGHV3.49, CPB2, CFP, GC, IGHG2, C8B, C4BPA, F12, 
CLEC3B, CFH.CFHR1, C1R, F13B, AHSG, IGHG3, APOD, KLKB1, C1S, CD5L, HPX, VTN, ATRN, JCHAIN, APOC3, IGHA2, IGHA1, 
IGHV3.15, IGHG1, IGFALS, ITIH3, SERPING1, SERPINA4, IGHM, ORM1.ORM2, F2, ACTB.ACTG1, RBP4, C1QA, C1QB, SERPINF2, 
IGKV2.30, IGHV1.2, C1RL, CPN1, SAA4, SAA1.SAA2, IGHG2.IGHG3, APOC1, HBB, ORM2, IGHA1.IGHA2, ECM1, FCN3, LGALS3BP, 
IGHG4, ORM1, APOA2, APOC2, F13A1, SERPINA10, PON1, SERPIND1, HABP2, HBD, SAA1, F9, GPLD1, HBA1, GPX3, LUM, C1QC, 
MBL2, TGFBI, PRG4, LYZ, PPBP, IGHV6.1, IGHV3.30.IGHV3.30.5, PZP, ACTBL2, SHBG, FETUB, CFHR2, IGLV3.19, CFHR5, HBB.HBD, 
APOM, S100A9, IGKV1.17, IGLV1.51, IGLV1.40, IGKV4.1, C4A, IGHV3.72, HPR, IGHV4.34.IGHV4.38.2, LCAT, CFHR1, IGLV3.21, IGHV1.69
 </pre>
</details>

- **12 Controls, 36 Cases (115 Excluded)**
 <details>
<summary>Group Exclusions</summary>
<br>Patients who become >5 and then go on to get worse (1) or better (0). Sample is first at which they are >5	
<br>
<pre>
| Aux.Id      | Group    | Reason for exclusion              |
|-------------|----------|-----------------------------------|
| C19-CB-0000 | Excluded | Incomplete data                   |
| C19-CB-0001 | Excluded | All points <=5                    |
| C19-CB-0003 | Excluded | All points <=5                    |
| C19-CB-0005 | Excluded | All points <=5                    |
| C19-CB-0008 | 0        |                                   |
| C19-CB-0009 | 1        |                                   |
| C19-CB-0010 | Excluded | All points <=5                    |
| C19-CB-0012 | 0        |                                   |
| C19-CB-0013 | 1        |                                   |
| C19-CB-0016 | 1        |                                   |
| C19-CB-0018 | Excluded | All points <=5                    |
| C19-CB-0020 | 0        |                                   |
| C19-CB-0021 | 0        |                                   |
| C19-CB-0022 | Excluded | All points <=5                    |
| C19-CB-0023 | Excluded | All points <=5                    |
| C19-CB-0025 | 1        |                                   |
| C19-CB-0026 | Excluded | All points <=5                    |
| C19-CB-0029 | Excluded | All points <=5                    |
| C19-CB-0030 | Excluded | All points <=5                    |
| C19-CB-0032 | 1        |                                   |
| C19-CB-0033 | 1        |                                   |
| C19-CB-0035 | Excluded | All points <=5                    |
| C19-CB-0036 | Excluded | Single time point                 |
| C19-CB-0037 | Excluded | All points <=5                    |
| C19-CB-0038 | Excluded | All points <=5                    |
| C19-CB-0039 | Excluded | All points <=5                    |
| C19-CB-0041 | Excluded | All points <=5                    |
| C19-CB-0042 | Excluded | All points <=5                    |
| C19-CB-0043 | Excluded | All points <=5                    |
| C19-CB-0044 | Excluded | All points <=5                    |
| C19-CB-0045 | Excluded | All points <=5                    |
| C19-CB-0046 | Excluded | All points <=5                    |
| C19-CB-0047 | Excluded | All points <=5                    |
| C19-CB-0048 | Excluded | All points <=5                    |
| C19-CB-0049 | Excluded | All points <=5                    |
| C19-CB-0050 | Excluded | All points <=5                    |
| C19-CB-0051 | Excluded | All points <=5                    |
| C19-CB-0052 | Excluded | All points <=5                    |
| C19-CB-0053 | Excluded | All points <=5                    |
| C19-CB-0054 | Excluded | All points <=5                    |
| C19-CB-0055 | Excluded | All points <=5                    |
| C19-CB-0056 | Excluded | All points <=5                    |
| C19-CB-0057 | Excluded | Incomplete data                   |
| C19-CB-0058 | 0        |                                   |
| C19-CB-0059 | 1        |                                   |
| C19-CB-0060 | Excluded | All points <=5                    |
| C19-CB-0061 | 1        |                                   |
| C19-CB-0062 | 0        |                                   |
| C19-CB-0063 | Excluded | All points <=5                    |
| C19-CB-0064 | 1        |                                   |
| C19-CB-0065 | Excluded | All points <=5                    |
| C19-CB-0066 | Excluded | All points <=5                    |
| C19-CB-0067 | Excluded | All points <=5                    |
| C19-CB-0068 | Excluded | All points <=5                    |
| C19-CB-0069 | Excluded | All points <=5                    |
| C19-CB-0070 | Excluded | All points <=5                    |
| C19-CB-0071 | Excluded | All points <=5                    |
| C19-CB-0072 | Excluded | All points <=5                    |
| C19-CB-0073 | Excluded | All points <=5                    |
| C19-CB-0075 | Excluded | All points <=5                    |
| C19-CB-0076 | 1        |                                   |
| C19-CB-0077 | Excluded | All points <=5                    |
| C19-CB-0078 | Excluded | All points <=5                    |
| C19-CB-0082 | 1        |                                   |
| C19-CB-0083 | Excluded | <=5 within 25 days but died       |
| C19-CB-0084 | Excluded | Withdrew consent                  |
| C19-CB-0085 | 1        |                                   |
| C19-CB-0086 | Excluded | All points <=5                    |
| C19-CB-0087 | Excluded | All points <=5                    |
| C19-CB-0088 | Excluded | All points <=5                    |
| C19-CB-0089 | Excluded | All points <=5                    |
| C19-CB-0090 | 1        |                                   |
| C19-CB-0091 | 0        |                                   |
| C19-CB-0092 | Excluded | All points <=5                    |
| C19-CB-0094 | Excluded | <=5 within 25 days but died       |
| C19-CB-0095 | Excluded | All points <=5                    |
| C19-CB-0096 | Excluded | admission dates missing           |
| C19-CB-0097 | Excluded | All points <=5                    |
| C19-CB-0098 | 1        |                                   |
| C19-CB-0099 | 1        |                                   |
| C19-CB-0100 | Excluded | All points <=5                    |
| C19-CB-0101 | Excluded | All points <=5                    |
| C19-CB-0102 | Excluded | Incomplete data                   |
| C19-CB-0103 | 1        |                                   |
| C19-CB-0104 | Excluded | Incomplete data                   |
| C19-CB-0106 | Excluded | Incomplete data                   |
| C19-CB-0107 | Excluded | All points <=5                    |
| C19-CB-0108 | 1        |                                   |
| C19-CB-0109 | 1        |                                   |
| C19-CB-0111 | Excluded | No outcome info                   |
| C19-CB-0112 | 1        |                                   |
| C19-CB-0113 | 1        |                                   |
| C19-CB-0114 | Excluded | All points <=5                    |
| C19-CB-0115 | Excluded | All points <=5                    |
| C19-CB-0116 | Excluded | Incomplete data                   |
| C19-CB-0117 | Excluded | All points <=5                    |
| C19-CB-0118 | Excluded | Incomplete data                   |
| C19-CB-0119 | Excluded | All points <=5                    |
| C19-CB-0120 | 1        |                                   |
| C19-CB-0121 | Excluded | All points <=5                    |
| C19-CB-0122 | Excluded | Single time point                 |
| C19-CB-0123 | 1        |                                   |
| C19-CB-0124 | 0        |                                   |
| C19-CB-0125 | Excluded | All points <=5                    |
| C19-CB-0126 | 0        |                                   |
| C19-CB-0127 | Excluded | Data doesn't extend 25 days       |
| C19-CB-0128 | Excluded | <=5 within 25 days but died       |
| C19-CB-0129 | Excluded | All points <=5                    |
| C19-CB-0130 | 1        |                                   |
| C19-CB-0131 | Excluded | All points <=5                    |
| C19-CB-0132 | Excluded | Refused treatment and died        |
| C19-CB-0133 | 1        |                                   |
| C19-CB-0134 | Excluded | All points <=5                    |
| C19-CB-0135 | 1        |                                   |
| C19-CB-0136 | 1        |                                   |
| C19-CB-0137 | 1        |                                   |
| C19-CB-0138 | Excluded | All points <=5                    |
| C19-CB-0139 | Excluded | All points <=5                    |
| C19-CB-0140 | Excluded | All points <=5                    |
| C19-CB-0141 | Excluded | All points <=5                    |
| C19-CB-0142 | 1        |                                   |
| C19-CB-0143 | Excluded | All points <=5                    |
| C19-CB-0144 | Excluded | All points <=5                    |
| C19-CB-0145 | Excluded | All points <=5                    |
| C19-CB-0147 | Excluded | All points <=5                    |
| C19-CB-0148 | Excluded | All points <=5                    |
| C19-CB-0149 | Excluded | All points <=5                    |
| C19-CB-0150 | 1        |                                   |
| C19-CB-0151 | Excluded | All points <=5                    |
| C19-CB-0152 | Excluded | All points <=5                    |
| C19-CB-0155 | Excluded | All points <=5                    |
| C19-CB-0157 | Excluded | All points <=5                    |
| C19-CB-0159 | 1        |                                   |
| C19-CB-0160 | Excluded | Single time point                 |
| C19-CB-0162 | 0        |                                   |
| C19-CB-0164 | 1        |                                   |
| C19-CB-0165 | 1        |                                   |
| C19-CB-0166 | Excluded | All points <=5                    |
| C19-CB-0167 | Excluded | All points <=5                    |
| C19-CB-0168 | Excluded | All points <=5                    |
| C19-CB-0169 | 1        |                                   |
| C19-CB-0170 | Excluded | Single time point/Incomplete data |
| C19-CB-0175 | Excluded | Incomplete data                   |
| C19-CB-0176 | 0        |                                   |
| C19-CB-0179 | Excluded | All points <=5                    |
| C19-CB-0180 | Excluded | All points <=5                    |
| C19-CB-0181 | Excluded | All points <=5                    |
| C19-CB-0196 | Excluded | All points <=5                    |
| C19-CB-0197 | Excluded | All points <=5                    |
| C19-CB-0198 | 0        |                                   |
| C19-CB-0199 | 1        |                                   |
| C19-CB-0214 | Excluded | Incomplete data                   |
| C19-CB-0215 | 1        |                                   |
| C19-CB-0216 | Excluded | All points <=5                    |
| C19-CB-0217 | Excluded | All points <=5                    |
| C19-CB-0218 | 1        |                                   |
| C19-CB-0219 | Excluded | All points <=5                    |
| C19-CB-0220 | Excluded | Refused treatment and died        |
| C19-CB-0221 | Excluded | All points <=5                    |
| C19-CB-0222 | Excluded | All points <=5                    |
| C19-CB-0223 | Excluded | All points <=5                    |
| C19-CB-0224 | Excluded | All points <=5                    |
| C19-CB-0225 | Excluded | Incomplete data                   |
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

## Detailed graphs for each type separately
### Model only on CLINICAL features
### Model only on PROTEINS features
### Model on CLINICAL & PROTEINS features

