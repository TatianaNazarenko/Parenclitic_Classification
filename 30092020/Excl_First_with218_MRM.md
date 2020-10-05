# EXCL/FIRST/WITH218/MRM

# Main analysis
![Image](ExclDNI_First_MRM_with_218_mainfig_MRM.png)

# Predcitions for "all network features" and "eweights only"
We are testing 5 models
- **glmnet** 
tunning parameters with cv on Train: alpha = seq(0, 1, length=10), lambda = seq(0.0001, 1, length = 100)
- **glmnet (fix alpha = 1)**
tunning parameters with cv on Train: alpha = 1, lambda = seq(0.0001, 1, length = 100)
- **glmnet (fix alpha = 0)**
tunning parameters with cv on Train: alpha = 0, lambda = seq(0.0001, 1, length = 100)
- **glmnet (fix alpha = 0.5)**
tunning parameters with cv on Train: alpha = 0.5, lambda = seq(0.0001, 1, length = 100)
- **Radial SVM**
tunning parameters with cv on Train: sigma= 2^c(-25, -20, -15,-10, -5, 0), C= 2^c(0:5)

## "all network features"
![Image](ExclDNI_First_all_features_MRM.png)

## "eweights only"
![Image](ExclDNI_First_Eweights_only_MRM.png)

# NETWORKS
![Image](ExclDNI_First_MRM_patients_networks.png)