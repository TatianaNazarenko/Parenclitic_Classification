# INCL/FIRST/WITH218/MRM

# Main analysis
![Image](InclDNI_First_MRM_title_fig.png)

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
![Image](InclDNI_First_MRM_all_features.png)

## "eweights only"
![Image](InclDNI_First_MRM_Eweights_only.png)

## "sds and means only only" (as the best for svm on l?ocv)
![Image](InclDNI_First_MRM_sds_and_mean_only.png)


# NETWORKS
![Image](InclDNI_First_MRM_patients_networks.png)
