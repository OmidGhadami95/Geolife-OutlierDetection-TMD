# Geolife-OutlierDetection-visualization-TMD
Outlier detection using IQR and Z-score, and also visualization on Geolife dataset for transport mode detection task
After loading and preprocessing the Geolife dataset, we have many CSVs, which include distance, velocity, acceleration, and ... as features (columns). The point is that some records are abnormal. For example, we have some records with more than 100 km/s velocity in the 'walk' label! Hence, it's crucial to remove these incorrect and noisy records. Otherwise, our network will train with inaccurate data, leading to lower accuracy. Moreover, Visualizing data before and after outlier detection is crucial for gaining insights into analyzing the effect of outlier detection. In this code, z-score and IQR have been used for outlier-detection
First, we must detect outliers and then remove all of them. Finally, all records after removing outliers must be merged.

Raw Geolife dataset link : https://download.microsoft.com/download/F/4/8/F4894AA5-FDBC-481E-9285-D5F8C4C4F039/Geolife%20Trajectories%201.3.zip

Notice:
Use IQR or z-score not both
Tune z-score hyperparameter (threshold)
This part must perform before calculating aggregated features
