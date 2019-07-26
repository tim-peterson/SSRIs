# SSRIs
CADs vs. non-CADs

`CADs <- read_csv("OneDrive-v2/Data/SSRIs/CADs_ge_v3_all_gene_CPM_avgs_only.csv")`

`View(CADs)`

`CADs_1 <- CADs[,-1]`

`CADs_1_t <- t(CADs_1)`

`autoplot(prcomp(CADs_1_t), data = CADs_1_t, label = TRUE)`
