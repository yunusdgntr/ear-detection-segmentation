# Efficient and Lightweight Ear Segmentation 

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<p>
  <img alt="Python38" src="https://img.shields.io/badge/Python-3.8-3776AB.svg?logo=Python&logoColor=white"></img>
  <img alt="Python39" src="https://img.shields.io/badge/Python-3.9-3776AB.svg?logo=Python&logoColor=white"></img>
  <img alt="Python310" src="https://img.shields.io/badge/Python-3.10-3776AB.svg?logo=Python&logoColor=white"></img>
  <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-v1.13.1-EE4C2C.svg?logo=PyTorch&logoColor=white"></img>
  <img alt="Torchvision" src="https://img.shields.io/badge/Torchvision-v0.14.1-EE4C2C.svg?logo=PyTorch&logoColor=white"></img>
  <img alt="Cuda" src="https://img.shields.io/badge/Cuda-Enabled-76B900.svg?logo=Nvidia&logoColor=white"></img>
  <img alt="Poetry" src="https://img.shields.io/badge/Poetry-60A5FA.svg?logo=Poetry&logoColor=white"></img>
  <img alt="Black" src="https://img.shields.io/badge/code%20style-black-black"></img>
  <img alt="Mypy" src="https://img.shields.io/badge/mypy-checked-blue"></img>
  <img alt="isort" src="https://img.shields.io/badge/isort-checked-yellow"></img>
</p>

## Download Model :open_file_folder:

<p>
<a href="https://drive.google.com/drive/folders/1l88PrrNESBDZ4Jd3QJSG9EbIe0CjXC_j?usp=sharing"><img alt="GoogleDrive" src="https://img.shields.io/badge/GoogleDrive-4285F4?logo=GoogleDrive&logoColor=white"></a>
<a href="https://github.com/umitkacar/Ear-segmentation-ai/releases/download/v1.0.0/earsegmentation_model_v1_46.pth"><img alt="Github" src="https://img.shields.io/badge/Github Download-181717?logo=Github&logoColor=white"></a>
</p>

## Requirements ⚙️

* Python 3.8 to Python3.10 (Virtualenv recommended)
* Download Ear Model file and put into `model_ear` folder
* Optional: poetry
* Optional: Nvidia CUDA for cuda usage

## :hammer_and_wrench: Installation :hammer_and_wrench:

### Pip installation :sparkles:

```properties
pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
```

### Poetry installation :sparkles:

```properties
poetry shell
poetry install
```

## Optional (If you have multiple python installation)

```properties
poetry env use $(which python3.10)
poetry shell
poetry install
```

## Usage

```
usage: earsegmentationai_cli.py [-h] -m {c,p} [-d [{cpu,cuda}]] [-fp FOLDERPATH] [-id [DEVICEID]]

options:
  -h, --help            show this help message and exit
  -m {c,p}, --mode {c,p}
                        Select camera or picture mode
  -d [{cpu,cuda}], --device [{cpu,cuda}]
                        Run in gpu or cpu mode
  -fp FOLDERPATH, --folderpath FOLDERPATH
                        Folder path for image(s) for image mode only
  -id [DEVICEID], --deviceId [DEVICEID]
                        Camera deviceId /dev/videoX for camera mode only
```

Webcam Mode :camera:

```properties
python earsegmentationai_cli.py --mode c --device gpu
```

Image Mode :art:

```properties
python earsegmentationai_cli.py --mode m --fp /path/xxx/
```

## Youtube Video :camera: :sparkles:

<p>
<a href="https://www.youtube.com/watch?v=5Puxj7Q0EEo"><img alt="Youtube" src="https://img.shields.io/badge/Youtube-FF0000?logo=Youtube&logoColor=white"></a>
</p>
