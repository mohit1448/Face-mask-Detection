# Face-mask-Detection

Input size of the model is 260x260, the backbone network only has 8 conv layers. The total model has only 24 layers with the  location and classification layers counted.

SSD anchor configurtion is show bellow:

| multibox layers | feature map size | anchor size | aspect ratio）|
| ---- | ---- | ---- | ---- |
|First|33x33|0.04,0.056|1,0.62,0.42|
Second ||17x17|0.08,0.11|1,0.62,0.42|
|Third|9x9|0.16,0.22|1,0.62,0.42|
|Forth |5x5|0.32,0.45|1,0.62,0.42|
|Fifth|3x3|0.64,0.72|1,0.62,0.42|

## How to run

on image：
```
python infer.py  --img-path /path/to/your/img
```
on video：
```
python infer.py --img-mode 0 --video-path /path/to/video  
# If you want to run with camera video, set  video_path to be 0
python infer.py --img-mode 0 --video-path 0
```


