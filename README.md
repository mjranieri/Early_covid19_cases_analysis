## Early COVID-19 cases analysis

This project performs a descriptive and epidemiological analysis of early
COVID-19 imported cases in China using publicly available case-level data from kaggle:

[COVID19_line_list_data.csv](https://storage.googleapis.com/kagglesdsdata/datasets/494724/994000/COVID19_line_list_data.csv?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=gcp-kaggle-com%40kaggle-161607.iam.gserviceaccount.com%2F20260201%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20260201T045617Z&X-Goog-Expires=259200&X-Goog-SignedHeaders=host&X-Goog-Signature=2457e40389a701d735401ac3a8583d7fbf255ff8995201cf4e794ed9567a083c60e9957762ff77970285eb59a68fa48a26e9e883a50df5221ef6b0d453bea90a44cb89653f4f69fc2189ee9354fde97c20c359066e09b91f475c70911fdf898c46a1c10407e035d50c896ce499d2a83174724c660002bd8e72e51ea79fac0bf767a8c39d80b5baad5445cdcd7c84f2a9baacaea1641458673ad0061687083d6e04380bc85ea7abfce5bd6e92437415168eadcccfff5832f193b2d1e4ee14842c0137ac9c53cad0f8ce811919b3ef9b54b8dc41109ba58d95c98f2e102d435772679ca9b65d1b795cbcbd87d827c20c0c9b00627ab3df69e42d3c6e9756b93a81)

### Contents
- Data cleaning and exploratory analysis
- Delay analysis between symptom onset, hospitalization, and reporting
- Geographic distribution of cases across Chinese provinces
- Logistic regression analysis of factors associated with mortality
- Limitations

### Methods
Analyses were conducted in R using the tidyverse ecosystem for data cleaning, transformation, and visualization. Temporal and demographic patterns were explored using ggplot2, while geographic distributions were analyzed using the sf package. Factors associated with mortality were investigated using generalized linear models with a binomial family (logistic regression). Age, gender, delay to hospitalization, and Wuhan-related exposure were included as covariates. Interaction terms were tested to assess potential effect modification, and results were interpreted using odds ratios with confidence intervals.

### Notes
Results reflect early epidemic dynamics and should be interpreted cautiously.
