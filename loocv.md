# DEATH 7, MRM (with super honnest LOOCV)

![Image](/docs/Aucs_pca.png)

## suggestions
* remove patients with _"Noch stationar"_ outcome (we don't know _our outcome_ for them!); recheck metadata for 0036, 0012, 0136 (look very strange);
* consider on FULL set (not only on MRM). We highlited [here](https://tatiananazarenko.github.io/Parenclitic_Classification/DEATH7.html) the best 15 proteins, but only 3 of them in MRM subset.

## Annotation for figures:
* If Group = 1 and prediction > 0.8 or Group = 0 and prediction < 0.2 -- GREEN display
* If Group = 1 and prediction < 0.2 or Group = 0 and prediction > 0.8 -- RED circle
* If NOCH Stationar and (Group = 1 and prediction < 0.5 or Group = 0 and prediction > 0.5) -- RED display

### Example for IncDNI_Imputation, LOOCV, betweenness, PCA
![Image](/docs/IncDNI_Imputation_LOOCV_betweenness_full.png)

### Example for IncDNI_Imputation, LOOCV, strength, PCA
![Image](/docs/IncDNI_Imputation_LOOCV_strength_full.png)

### Example for IncDNI_NoImputation, LOOCV, betweenness, PCA
![Image](/docs/IncDNI_NoImputation_LOOCV_betweenness_full.png)

### Example for IncDNI_NoImputation, LOOCV, strength, PCA
![Image](/docs/IncDNI_NoImputation_LOOCV_strength_full.png)


