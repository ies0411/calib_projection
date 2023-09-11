#readme

# Projection Visualizer 2D, 3D

## Index

- [Overall](#overall)
- [Dependancy](#Dependancy)
- [Install](#Install)
- [Parameter](#Parameter)
- [Demo](#Demo)

---

## Overall

In order to calibrate multi sensor, you need to check whethere the result(Extrinsic Parameter) is correct or not. And, It is much more convenience in headless env. This projection is for that case. You can employ this project when you make your 2D/3D result visualize.
All you need is just jupyter-notebook.

## Dependancy

- python 3.7 or up
- Opencv 3.4 or up
- Open3D 0.15 (lastest realease)

## Install

- open3D

```
# Install
pip install open3d

# Verify installation
python -c "import open3d as o3d; print(o3d.__version__)"

# Python API
python -c "import open3d as o3d; \
           mesh = o3d.geometry.TriangleMesh.create_sphere(); \
           mesh.compute_vertex_normals(); \
           o3d.visualization.draw(mesh, raw_mode=True)"

# Open3D CLI
open3d example visualization/draw

```

## Parameter

1. Kitti

```
lidar_path = '(YOUR KITTI LIDAR FILE PATH)/(FILE NAME).bin'
img_path = '(YOUR KITTI IMG FILE PATH)/(FILE NAME)'
v2c_filepath = '(YOUR KITTI CALIB FILE PATH)/calib_velo_to_cam.txt'
c2c_filepath = '(YOUR KITTI CALIB FILE PATH)/calib_cam_to_cam.txt'
```

2. Kitti 360

```
lidar_path = '(YOUR KITTI360 LIDAR FILE PATH)/(FILE NAME).bin'
img_path = '(YOUR KITTI360 LIDAR FILE PATH)/(FILE NAME)'
v2c_filepath = '(YOUR KITTI360 LIDAR FILE PATH)/calib_cam_to_velo.txt'
c2c_filepath = '(YOUR KITTI360 LIDAR FILE PATH)/perspective.txt'
```

3. Open3D

```
TODO
```

## Demo

### TODO : change img, color, refer to KITTI TUTORIAL

1. Kitti

Download link : [Kitti](http://www.cvlibs.net/datasets/kitti/raw_data.php)

![output](https://user-images.githubusercontent.com/44966311/182513983-506cbcb1-34fd-4c02-b8cd-c82ab8b697a7.png)

2. Kitti 360

Download link : [Kitti](http://www.cvlibs.net/datasets/kitti/raw_data.php)

![output_360](https://user-images.githubusercontent.com/44966311/182514306-50bbcba5-d13e-4774-a1a4-1687e7919e4c.png)

3. Open3D

![Screenshot from 2022-08-03 11-54-33](https://user-images.githubusercontent.com/44966311/182514130-d3c7b2bd-3d8b-42ca-99d0-7d7c611661ba.png)

---

## Authors

- **Eunsoo Im** - <eslim@superb-ai.com>
- sensor fusion | 3D vision engineer in Superb-AI co.

See also the list of [contributors](https://github.com/always0ne/readmeTemplate/contributors)
who participated in this project.

<!--
## Used or Referenced Projects
 - [referenced Project](project link) - **LICENSE** - little-bit introduce
-->

## License

```
MIT License

Copyright (c) 2022 voda

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
