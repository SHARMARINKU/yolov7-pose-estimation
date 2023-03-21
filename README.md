"""
Yolo v7-Pose-Estimation


Author: Rinku Sharma
E-mail: rinkusharma1466@gmail.com

This file handles and detect the human key point which is (x,y,keypoint) it will return 51 values.
"""

```
cd yolov7-pose-estimation
```

- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)
```
### For Linux Users
python3 -m venv psestenv
source psestenv/bin/activate

### For Window Users
python3 -m venv psestenv
cd psestenv
cd Scripts
activate
cd ..
cd ..
```

- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```

- Install requirements with mentioned command below.

```
pip install -r requirements.txt
```

- Download yolov7 pose estimation weights from [link](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-w6-pose.pt) and move them to the working directory {yolov7-pose-estimation}


- Run the code with mentioned command below.
```
python pose-estimate.py

#if you want to change source file
python pose-estimate.py --source "your custom video.mp4"

#For CPU
python pose-estimate.py --source "your custom video.mp4" --device cpu

#For GPU
python pose-estimate.py --source "your custom video.mp4" --device 0

#For View-Image
python pose-estimate.py --source "your custom video.mp4" --device 0 --view-img

#For LiveStream (Ip Stream URL Format i.e "rtsp://username:pass@ipaddress:portno/video/video.amp")
python pose-estimate.py --source "your IP Camera Stream URL" --device 0 --view-img

#For WebCam
python pose-estimate.py --source 0 --view-img

#For External Camera
python pose-estimate.py --source 1 --view-img
```

- Output file will be created in the working directory with name <b>["your-file-name-without-extension"+"_keypoint.mp4"]</b>

#### RESULTS

<table>
  <tr>
    <td>Football Match Pose-Estimation</td>
     <td>Cricket Match Pose-Estimation</td>
     <td>FPS and Time Comparision</td>
     <td>Live Stream Pose-Estimation</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/62513924/image1.png" width=640 height=180></td>
    <td><img src="https://user-images.githubusercontent.com/62513924/185228806-4ba62e7a-12ef-4965-a44a-6b5ba9a3bf28.png" width=640 height=180></td>
    <td><img src="https://user-images.githubusercontent.com/62513924/185324844-20ce3d48-f5f5-4a17-8b62-9b51ab02a716.png" width=640 height=180></td>
    <td><img src="https://user-images.githubusercontent.com/62513924/185587159-6643529c-7840-48d6-ae1d-2d7c27d417ab.png" width=640 height =180></td>
  </tr>
 </table>


# yolov7-pose-estimation
# yolov7-pose-estimation
