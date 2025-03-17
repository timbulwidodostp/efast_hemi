# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Exploratory Factor Analysis with Structured Residuals Use efast_hemi (efast) With (In) R Software
install.packages("remotes")
remotes::install_github("vankesteren/efast")
library("efast")
efast_hemi = read.csv("https://raw.githubusercontent.com/timbulwidodostp/efast_hemi/main/efast_hemi/efast_hemi.csv",sep = ";")
# Estimation Exploratory Factor Analysis with Structured Residuals Use efast_hemi (efast) With (In) R Software
efast_hemi <- efast_hemi(data = efast_hemi, M = 4, lh_idx = 1:17, rh_idx = 18:34)
Loadings <- efast_loadings(efast_hemi, symmetry = TRUE)
lateralization <- lateralization(efast_hemi)
efast_hemi
Loadings
lateralization
# Exploratory Factor Analysis with Structured Residuals Use efast_hemi (efast) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished