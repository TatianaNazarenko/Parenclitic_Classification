### Last Results (14.08.2020)
# Lasso regression with LOOCV

<details>
  <summary>WORSE/BETTER</summary>
  <br>
  <pre>
    | Type                 | AUC (95% CI)        | Final model                                |
    |----------------------|---------------------|--------------------------------------------|       
    | proteomic            | 0.729 (0.540-0.917) | PGLYRP2, KLKB1.                            |

  </pre>
</details>

<details>
  <summary>WORSE/BETTER</summary>
  <br> (the same as the previous one)
  <br>
  <pre>
    | Type                 | AUC (95% CI)        | Final model                                |
    |----------------------|---------------------|--------------------------------------------|       
    | proteomic            | 0.729 (0.540-0.917) | PGLYRP2, KLKB1.                            |

  </pre>
</details>
 
<details>
  <summary>DEATH 5</summary>
  <br>
  <pre>
    | Type                 | AUC (95% CI)        | Final model                                |
    |----------------------|---------------------|--------------------------------------------|
    | clinical             | 0.854 (0.763-0.944) | N.PH, N.LAC                                |        
    | proteomic            | 0.864 (0.776-0.953) | HRG, SERPINA3, FETUB, MASP2                |
    | clinical &  proteomic| 0.917 (0.851-0.983) | N.PH, N.LAC, SERPINA3, MASP2               |
  </pre>
</details>

<details>
  <summary>DEATH 6</summary>
  <br>
  <pre>
    | Type                 | AUC (95% CI)        | Final model                                |
    |----------------------|---------------------|--------------------------------------------|
    | clinical             | 0.870 (0.779-0.961) | N.PH, N.LAC                                |        
    | proteomic            | 0.878 (0.779-0.976) | KNG1, CFI, HRG, SERPINA3, FETUB, MASP2     |
    | clinical &  proteomic| 0.917 (0.849-0.986) | N.PH, N.LAC, SERPINA3, MASP2.              |
  </pre>
</details>

<details>
  <summary>DEATH 7</summary>
  <br>
  <pre>
    | Type                 | AUC (95% CI)        | Final model                                |
    |----------------------|---------------------|--------------------------------------------|
    | clinical             | 0.844 (0.732-0.956) | N.PCO2, N.PH, N.LAC                        |        
    | proteomic            | 0.900 (0.816-0.985) | A2M, KNG1, CFI, HRG, PZP, SERPINA3, MASP2  |
    | clinical &  proteomic| 0.897 (0.806-0.987) | N.PCO2, N.PH, N.LAC, MASP2                 |
  </pre>
</details>



# Parenclitic Models

(_for these versions we use only **clinical &  proteomic** type_ )
- [WORSE/BETTER](A.md)
- [WORSE/BETTER (with AGE)](WA.md)
- [DEATH 5](DEATH5.md)
- [DEATH 6](DEATH6.md)
- [DEATH 7](DEATH7.md)
- [COMMON DEATH](COMMON_DEATH.md)
