# 使用说明

## 环境依赖

升级显卡驱动，支持到cuda>=12.1

python==3.10.6

torch==2.1.2+cu121

torchvision=0.16.2+cu121

requests

opencv-python

loguru

gradio==3.4.1

httpx==0.24.1

k_diffusion

pynvml

omegaconf

diffusers

transformers

pytorch_lightning

numba

## 预训练模型

将SD的预训练权重sd-v1-4.ckpt，重命名为model.ckpt，并放置在models/ldm/stable-diffusion-v1文件夹下

将Bert的预训练权重Clip-Vit-Large-Patch14文件夹整个放在models文件夹下 

## 运行

运行scripts文件夹下的webui.py，运行成功会出现下面的提示：

Running on local URL:  http://0.0.0.0:7860

7860为端口。

此时需要在cmd运行ipconfig命令，找到IPv4 地址，例如123.45.678.123

然后打开浏览器，输入http://123.45.678.123:7860，即可运行webui。

## 说明
项目整体来源于：https://github.com/Sygil-Dev/sygil-webui.git

当前只保证了文生图功能是正常的，由于删除了“我认为”的一些冗余代码，所以不能保证其他功能是否也正常。