# Geolife-OutlierDetection-TMD
Outlier detection for Geolife dataset for transport mode detection task
After loading and preprocessing the Geolife dataset, we have some csv which include distance, velocity, acceleration, and ... columns. The point is, some records are abnormal. For example, we have some records in 'walk' label which have 100 km/s velocity! So, it's crucial to remove these false records. Otherwise, our network will train with false data which leads to lower accuracy at the end.
First, we must detect outliers and then remove all of them. Finally, all records after removing outliers must be merged.
