# Apple LiDAR Pavement Cracks Dataset

## Overview
This dataset contains pavement crack point clouds collected using Apple LiDAR on an iPad 21 Pro at Sun Yat-sen University, Zhuhai Campus. The dataset is intended for research on the potential application of Apple LiDAR in pavement crack detection.

## Data Collection Details
- **Device**: iPad 21 Pro  
- **Software**: SiteScape  
- **Point Cloud Density**: Premium  
- **Point Cloud Size**: Small  
- **File Format**: .ply  
- **Each File Represents**: A single crack  

## Crack Measurement Attributes
- **Measurement Tool**: A vernier caliper with a resolution of **0.01mm** was used to measure crack width and depth.  
- **Crack Type Annotation**: Crack types (**transverse, longitudinal, alligator, and block cracks**) were manually labeled based on visual inspection.  
- **Measurement Variability**: Due to different crack characteristics, some width measurements represent average values.  
- **Weather Conditions**: Data was collected during **light rain**, and the point cloud may include water accumulation in cracks.  
- **Measurement Consistency**: All measurements were conducted by the **same team** to ensure consistency.  

## 📍 Crack Collection Locations
The image below shows the collection locations of different point cloud samples:

![Crack Collection Locations](location_map.jpg)

## Dataset Download
The full dataset (~40GB) is available for download from an external source due to its large size.

| Crack ID  | Crack Type  | Crack Width    | Crack Length | Crack Depth       | Download Link  |
|-----------|------------|---------------|--------------|-------------------|---------------|
| sysu001   | Longitudinal | 4-14mm       | 5.91m       | 50-90mm          | [Download](https://zenodo.org/records/14965713/files/sysy001.ply?download=1&preview=1) |
| sysu002   | Transverse  | 4.4mm        | 3.47m       | 10-50mm          | [Download](https://zenodo.org/records/14965713/files/sysu002.ply?download=1&preview=1) |
| sysu003   | Transverse  | 4-14mm       | 3.5m        | 10-30mm          | [Download](#) |
| sysu004   | Transverse  | 19-31mm      | 9m          | 6-20mm           | [Download](#) |
| sysu005   | Transverse  | 5-7mm        | 11.14m      | 50-100mm & >100mm | [Download](#) |
| sysu006   | Transverse  | 15-23mm      | 12.09m      | 15-35mm          | [Download](#) |
| sysu007   | Transverse  | Avg. 30mm    | 11.61m      | 20-40mm          | [Download](#) |
| sysu008   | Transverse  | 23-37mm      | 11.78m      | >10mm            | [Download](#) |
| sysu009   | Transverse  | 17mm         | 11.86m      | 10-40mm          | [Download](#) |
| sysu010   | Alligator   | Max 100mm    | 1.77m       | <17mm            | [Download](#) |
| sysu011   | Longitudinal | 1.5-20mm    | 5m          | 3-14mm           | [Download](#) |
| sysu012   | Longitudinal | >1mm        | 4.87m       | 10mm             | [Download](#) |
| sysu013   | Transverse  | 3-14mm       | 12.11m      | Max 20mm         | [Download](#) |

## Usage Instructions
- **Viewing**: You can use CloudCompare, MeshLab, or Open3D to visualize and analyze the point cloud data.
- **Processing**: Python users can load the `.ply` files with Open3D:
  ```python
  import open3d as o3d
  pcd = o3d.io.read_point_cloud("crack_001.ply")
  o3d.visualization.draw_geometries([pcd])
  ```

## Citation
If you use this dataset in your research, please cite appropriately:
> Apple LiDAR Pavement Cracks Dataset, Sun Yat-sen University, Zhuhai Campus

## License
This dataset is provided for research purposes only. Please contact the dataset owner for any commercial use inquiries.
