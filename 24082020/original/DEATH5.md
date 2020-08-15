 
# DEATH 5 (original)
 
## Data: 
- **203 Features**
<details>
<summary>Clinical (15)</summary>
 <pre>
I.Age, charlson, N.THROMBOZYTEN, N.GOT..AST..HP, N.GPT..ALT..HP, N.LDH.HP, N.CRP.HP, N.FERRITIN.HP,
N.PROCALCITONIN, N.INR, N.QUICK..TPZ., N.CREATINKINASE..CK..HP, N.KREATININ..JAFFe..HP, 
N.UNREIFE.GRANULOZYTEN.ABSOLUT, N.APTT
 </pre>
</details>
<details>
<summary>Proteins (188)</summary>
 <pre>
C4A.C4B, ALB, TTR, MST1, MASP1, ITIH1, IGLC7, A2M, C7, APOB, KNG1, APOE, C3, FN1, CFI, F10, PIGR, SERPINC1, 
IGLC7.IGLL5, HRG, SERPINA3, TF, IGLC2.IGLC3, IGKC, ITIH4, C8G, ITIH2, IGHV3.23, IGHV3.64D, CP, SELL, C4B, C9, 
AFM, CST3, C5, AMBP, CD14, VWF, A2M.PZP, GSN, FCGBP, IGHV3.13, CFH, AZGP1, ACTA2.ACTB.ACTG1.ACTG2, CPN2, PGLYRP2, 
IGLL5, APOA1, FGB, CFB, FGG, FBLN1, C6, APOA4, C8A, CNDP1, LRG1, CRP, C4BPB, S100A8, IGHG1.IGHG3, AGT, F11, 
CD44, FGA, SERPINF1, APOL1, SERPINA7, APOH, IGHV5.51, PROS1, IGHV1.18, IGKV1.5, IGKV3.20, CLU, LBP, CFD, PLG, 
LPA, A1BG, HP, HP.HPR, SERPINA1, C2, SERPINA6, F5, IGHV3.49, CPB2, CFP, GC, IGHG2, C8B, C4BPA, F12, CLEC3B, 
CFH.CFHR1, C1R, F13B, AHSG, IGHG3, APOD, KLKB1, C1S, CD5L, HPX, VTN, ATRN, JCHAIN, APOC3, IGHA2, IGHA1, IGHV3.15, 
IGHG1, IGFALS, ITIH3, SERPING1, SERPINA4, IGHM, ORM1.ORM2, F2, ACTB.ACTG1, RBP4, C1QA, C1QB, SERPINF2, IGKV2.30, 
IGHV1.2, C1RL, CPN1, SAA4, SAA1.SAA2, IGHG2.IGHG3, APOC1, HBB, ORM2, IGHA1.IGHA2, ECM1, FCN3, LGALS3BP, IGHG4, 
ORM1, APOA2, APOC2, F13A1, SERPINA10, PON1, SERPIND1, HABP2, HBD, SAA1, F9, GPLD1, HBA1, GPX3, LUM, C1QC, MBL2, 
TGFBI, PRG4, LYZ, PPBP, IGHV6.1, IGHV3.30.IGHV3.30.5, PZP, ACTBL2, SHBG, IGHV3.74, CFHR2, IGLV3.19, CFHR5, HBB.HBD, 
APOM, S100A9, IGKV1.17, IGLV1.51, IGLV1.40, IGKV4.1, C4A, IGHV3.72, HPR, IGHV4.34.IGHV4.38.2, LCAT, CFHR1, IGLV3.21, 
B2M, IGHV1.69
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

## Detailed graphs for each type separately
### Model only on CLINICAL features
### Model only on PROTEINS features
### Model on CLINICAL & PROTEINS features

