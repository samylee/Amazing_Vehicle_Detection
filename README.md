# Amazing_Vehicle_Detection
CPU Real-time Amazing Vehicle Detection
# Test steps
## step1
Download opencv_dll(`ours`) and put it to current directory [BaiDu Cloud](https://pan.baidu.com/s/1veDxI7dquI_ZPFctC6hpiA), password: weqv
## step2
Set parameters:
`Amazing_Vehicle_Detection.exe test_type img_path`
```cpp
like:  Amazing_Vehicle_Detection.exe image test.jpg  (for image)
or:    Amazing_Vehicle_Detection.exe imgdir /img/path/test_imgs  (for imgdir)
or:    Amazing_Vehicle_Detection.exe video test.avi  (for video)
or:    Amazing_Vehicle_Detection.exe video 0  (for usbcam)
```
# Algorithm efficiency
| Algorithm | min_size | COCO2014-AP | CPU(i7-9700K @3.6GHz) Speed/FPS |
|:------:|:------:|:------:|:------:|
| YOLO-V3-416x416  | 12x12 | 0.5002(thresh-0.5, IOU-0.5) |526ms/1.9|
| ours  | 12x12 | 0.4964(thresh-0.6, IOU-0.5) |46ms/21.7|
# Tips
1. 'Vehicle' include car+bus+truck.  
2. The image zooms to 608 by default, so if you want to test larger size pictures, please contact the author.
# Example result
![image](https://github.com/samylee/Amazing_Vehicle_Detection/blob/master/result/3.jpg)
# Reference
https://blog.csdn.net/samylee
