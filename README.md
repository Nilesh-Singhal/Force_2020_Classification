# Force_2020_Classification
Check out my solution for FORCE 2020 Lithology Classification Contest. The objective of the competition is to create machine learning model to correctly predict lithology labels using provided well logs, provided NPD Lithostratigraphy and well location X,Y position. Contest Link:- https://github.com/bolgebrygg/Force-2020-Machine-Learning-competition/tree/master/lithology_competition

I have used the following strategy for my solution:-

1. Clustering Based on Spatial Location
2. Missing Data Flags
3. Interpolated Zone Flags
4. Despiking of the logs
5. Flagging Bad Holes
6. Train and fill the flagged zones
7. Outlier Analysis
8. Feature Engineering
9. Dimensionality Reduction
10. Final Lithology Classification

Despiking of the log values has been done by using the threshold available in literature and from the statistical nature of data. Bad holes are flagged by comparing Caliper and Borehole Size log and by Using ensemble modeling for DTC and comparing the predicted DTC with actual log values to flag bad hole. Median Filter is used to denoise the features and new features such as Shale Volume and Carbon Index are also added.
