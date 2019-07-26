# SSRIs
CADs vs. non-CADs

`CADs <- read_csv("OneDrive-v2/Data/SSRIs/CADs_ge_v3_all_gene_CPM_avgs_only.csv")`

`View(CADs)`

`CADs_1 <- CADs[,-1]`

`CADs_1_t <- t(CADs_1)`

`autoplot(prcomp(CADs_1_t), data = CADs_1_t, label = TRUE)`


## hierarchal clustering [from here](https://dataaspirant.com/2018/01/08/hierarchical-clustering-r/)

`CADs_1_t <- na.omit(CADs_1_t)`

`CADs_1_t <- scale(CADs_1_t)`

[//]: # Dissimilarity matrix

`d <- dist(df, method = "euclidean")`

[//]: # Hierarchical clustering using Complete Linkage

`hc1 <- hclust(d, method = "complete" )`

[//]: # Plot the obtained dendrogram

`plot(hc1)`
