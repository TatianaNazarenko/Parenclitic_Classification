# DEATH 7, MRM (with super honnest LOOCV)

* For each characteristic (_autority_score, betweenness, closenness, edge_betweenness, eigen_centrality, page.rank, strength_) now we consider not the accumulating values, but the whole vectors.

_For example, for the strength characterisitc  (the strength of the vertices), we are considering not zeros, mean, maximum, minimum, sd, but for each patient we obtain the strength vector for all vertices._
* Then, on the training set (all points without one), we construct the PCA on a matrix consisting of all weights and create glm model on two principal components.
We apply to test point all pmodels (SVM, PCA, glm)

![Image](/docs/Aucs_pca.png)

## suggestions
* remove patients with _"Noch stationar"_ outcome (we don't know _our outcome_ for them!); recheck metadata for 0036, 0012, 0136 (look very strange);
* consider on FULL set (not only on MRM). We highlited [here](https://tatiananazarenko.github.io/Parenclitic_Classification/DEATH7.html) the best 15 proteins, but only 3 of them in MRM subset.

## Annotation for figures:
* If Group = 1 and prediction > 0.8 or Group = 0 and prediction < 0.2 -- GREEN display
* If Group = 1 and prediction < 0.2 or Group = 0 and prediction > 0.8 -- RED circle
* If NOCH Stationar and (Group = 1 and prediction < 0.5 or Group = 0 and prediction > 0.5) -- RED display

## NoImputation (betweenness, strength)

### Example for IncDNI_NoImputation, LOOCV, betweenness, PCA
![Image](/docs/IncDNI_NoImputation_LOOCV_betweenness_full.png)

### Example for IncDNI_NoImputation, LOOCV, strength, PCA
![Image](/docs/IncDNI_NoImputation_LOOCV_strength_full.png)

### Example C19-CB-0176 experiment (betweenness, strength)
#### betweenness
![Image](/docs/EXAMPLE_IncDNI_NoImputation_LOOCV_betweenness_C19-CB-0176_full.png)
#### strength
![Image](/docs/EXAMPLE_IncDNI_NoImputation_LOOCV_strength_C19-CB-0176_full.png)

### Example C19-CB-0220 experiment (betweenness, strength)
#### betweenness
![Image](/docs/EXAMPLE_IncDNI_NoImputation_LOOCV_betweenness_C19-CB-0220_full.png)
#### strength
![Image](/docs/EXAMPLE_IncDNI_NoImputation_LOOCV_strength_C19-CB-0220_full.png)

### Example for IncDNI_Imputation, LOOCV, betweenness, PCA
![Image](/docs/IncDNI_Imputation_LOOCV_betweenness_full.png)

### Example for IncDNI_Imputation, LOOCV, strength, PCA
![Image](/docs/IncDNI_Imputation_LOOCV_strength_full.png)




