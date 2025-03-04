# Apple LiDAR Pavement Cracks Dataset

## Overview
This dataset contains pavement crack point clouds collected using Apple LiDAR on an iPad 21 Pro at Sun Yat-sen University, Zhuhai Campus. The dataset is intended for research on the potential application of Apple LiDAR in pavement crack detection.

## Data Collection Details
- **Device**: iPad 21 Pro  
- **Software**: SiteScape  
- **Point Cloud Density**: Premium  
- **Point Cloud Size**: Small  
- **Coordinate System**: WGS84  
- **File Format**: .ply  
- **Each File Represents**: A single crack  
- **Additional File**: Location map showing different point cloud collection positions  

## Dataset Download
The full dataset (~40GB) is available for download from an external source due to its large size.

| File Name         | Description                         | Download Link |
|------------------|---------------------------------|---------------|
| sysu001.ply    | Pavement crack sample 001       | [Download](#) |
| sysu002.ply    | Pavement crack sample 002       | [Download](#) |
| ...              | ...                             | ...           |
| location_map.png | Point cloud collection locations | [Download](#) |
| sample_data.zip  | Sample dataset for quick access | [Download](#) |

## 📍 采集位置图
下图展示了不同点云数据的采集位置：

![采集位置图](location_map.jpg)


## Usage Instructions
- **Viewing**: You can use CloudCompare, MeshLab, or Open3D to visualize and analyze the point cloud data.
- **Processing**: Python users can load the `.ply` files with Open3D:
  ```python
  import open3d as o3d
  pcd = o3d.io.read_point_cloud("crack_001.ply")
  o3d.visualization.draw_geometries([pcd])
  ```
- **Coordinate System**: Data is aligned using WGS84 for accurate geolocation.

## Citation
If you use this dataset in your research, please cite appropriately:
> Apple LiDAR Pavement Cracks Dataset, Sun Yat-sen University, Zhuhai Campus

## License
This dataset is provided for research purposes only. Please contact the dataset owner for any commercial use inquiries.
