## Requirements
* Anaconda (if you haven't installed before)
  * for reference: https://blog.csdn.net/mouse2018/article/details/125125916
  * latest version: https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/Anaconda3-2023.07-2-MacOSX-arm64.pkg
* python >= 3.8
    * `conda create --name lightpose python==3.9`
    * `conda activate lightpose`
* `pip install -r requirements.txt`
  * torch>=0.4.1
  * torchvision>=0.2.1
  * pycocotools>=2.0.0 
  * opencv-python>=3.4.0.14 
  * numpy>=1.14.0
## Testing
* Currently only support `.mp4`
* Already set the pytorch to use GPU acceleration on Mac, no additional configuration required.
* At the repository root： \
`python demo.py --checkpoint-path ~/YOUR_PATH_TO/lightweight-human-pose-estimation.pytorch/data/checkpoint_iter_370000.pth --video PATH_TO_THE_VIDEO/video.mp4` 
* Output dir is set to `./data/` and video name is `output.mp4`, you can change it in `demo.py` at `line 94`
* Time cost will be shown in the console right after the test is done
  * Example: `--- 145.10227727890015 seconds ---`