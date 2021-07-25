# Unspervised-learning-on-NBA-data-k-means-
The goal is to group NBA players from 2017-2020 seasons by stats per 100 posseions. This way of collecting data don't has outliers and don't depend on minutes that players played.
# Data
Data came from https://www.basketball-reference.com. I drop rows with NaN and also filter fo players that played at least 540 minutes.
# Droping dependent scaled variables
![image](https://user-images.githubusercontent.com/62485500/126896560-b430e331-4728-4754-9899-ad8be9d05af9.png)

According to this matrix and my experince I left variables 2P, 3P, FT, ORB, DRB, AST, STL, BLK, PF.
# Elbow method
![image](https://user-images.githubusercontent.com/62485500/126896756-2008cd5b-935b-4855-ad16-7cfba2b65101.png)

Using elbow method doesn't show cleary number of clusters.
# PCA method for 2d visualization
![image](https://user-images.githubusercontent.com/62485500/126896787-fcb98ef6-a344-4eb0-a852-34e1e4ff95c6.png)

After testing 2d visualization i choose 4 as number of clusters, becouse we can see clearly diffrent clusters same as with 3 but we can get diferentiate players better. On 2d visualization for 5 clusters we can't see all clearly different clusters anymore.
# Number of players in each cluster with hue equals player position
![image](https://user-images.githubusercontent.com/62485500/126896965-3b917a3f-5f01-40ad-86e0-5c42ecde6dd0.png)

Here we can see how many players from each postion fall into each cluster
# Radar charts for each cluster
Cluster 0: Floor generals

![image](https://user-images.githubusercontent.com/62485500/126897110-67ba5c4f-5533-48a8-9158-03be25969f7a.png)

Cluster 1: Role players

![image](https://user-images.githubusercontent.com/62485500/126897113-8b3e1c0b-7ea0-4f8d-908d-6647a520412d.png)

Cluster 2: Bigs

![image](https://user-images.githubusercontent.com/62485500/126897116-fd5a6788-e612-421e-97a1-765339700edb.png)

Cluster 3: 3-pointers specialists

![image](https://user-images.githubusercontent.com/62485500/126897120-8f3f997d-0d53-492b-b9b0-7f786fec2a72.png)

# Cons of this approach
-We don't necessarily want approximately equal number of players in each group,

-K-means gives best results for highly varied observations, on 2d visualization we can clearly see less varied observations in bottom-left corner of chart.


