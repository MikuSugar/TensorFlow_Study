# 安装
## MAC（m1）安装
### 系统要求
MAC OS 12.0+
### 安装步骤
+ [下载Conda Env](https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh)
+ install Conda:
  ```bash
  chmod +x ~/Downloads/Miniforge3-MacOSX-arm64.sh
  sh ~/Downloads/Miniforge3-MacOSX-arm64.sh
  source ~/miniforge3/bin/activate
  ``` 
+ Install the Tensorflow dependencies:
  ```bash
  conda install -c apple tensorflow-deps
  ```
+ Install base tensorflow:
  ```bash
  python -m pip install tensorflow-macos
  ```
+ Install metal plugin:
  ```bash
  python -m pip install tensorflow-metal
  ```
### 目前的缺陷（不支持的部分）
+ Multi-GPU support
+ Acceleration for Intel GPUs
+ V1 TensorFlow Networks

### 参考
[https://developer.apple.com/metal/tensorflow-plugin/](https://developer.apple.com/metal/tensorflow-plugin/)
