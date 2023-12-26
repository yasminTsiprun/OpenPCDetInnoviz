# OpenPCDetInnoviz
car detection network. TRained in openpcdet frame work, using PVRECNN model and Innoviz point cloud.
We used point cloud which were acquired by Lidar sensor: InnovizOne.
InnovizOne is resilient to sunlight and weather conditions, and is able to deliver a rich 3D point cloud at distances up to 250 meters. 
The maximum FOV is 115〖115〗^0 x〖25〗^0 with frame rate of 10-15 FPS.

GPU resources:  2 NVIDIA GeForce RTX 2080 Ti graphics cards
Operation System: Ubuntu 20.04.6 LTS

253 point clouds were used for training and test.
51 point clouds were used validation

Dataset:
Folder Name	#Frames	#pcd files	Label counter
2023-03-26-18-53-51_static	4	4	48
2023-03-26-19-28-24_B_MovingSingleCarInParking	100	100	1269
2023-03-26-19-46-19_A	54	54	439
2023-03-26-19-46-19_end	34	34	109
2023-03-26-19-49-25_A	39	39	121
2023-03-26-19-49-25_C	22	22	224
2023-03-26-19-52-04_A	54	54	476


Resuls:
2023-11-20 18:25:55,703   INFO  *************** Performance of EPOCH 80 *****************
2023-11-20 18:25:55,703   INFO  Generate label finished(sec_per_example: 0.3311 second).
2023-11-20 18:25:55,704   INFO  recall_roi_0.3: 0.991111
2023-11-20 18:25:55,704   INFO  recall_rcnn_0.3: 0.993333
2023-11-20 18:25:55,704   INFO  recall_roi_0.5: 0.964444
2023-11-20 18:25:55,704   INFO  recall_rcnn_0.5: 0.962222
2023-11-20 18:25:55,704   INFO  recall_roi_0.7: 0.813333
2023-11-20 18:25:55,704   INFO  recall_rcnn_0.7: 0.900000
2023-11-20 18:25:55,704   INFO  Average predicted number of objects(51 samples): 8.647

