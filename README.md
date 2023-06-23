# Geolife-OutlierDetection-TMD
Outlier detection for Geolife dataset for transport mode detection task
After loading and preprocessing the Geolife dataset, we have some csv which include distance, velocity, acceleration, and ... columns. The point is, some records are abnormal. For example, we have some records in 'walk' label which have 100 km/s velocity! So, it's crucial to remove these false records. Otherwise, our network will train with false data which leads to lower accuracy at the end.
First, we must detect outliers and then remove all of them. Finally, all records after removing outliers must be merged.


Raw Geolife dataset link : https://download.microsoft.com/download/F/4/8/F4894AA5-FDBC-481E-9285-D5F8C4C4F039/Geolife%20Trajectories%201.3.zip

preprocess code will be added soon.
