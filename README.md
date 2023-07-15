# Windows端本地配置stable diffusion

### 本地环境

intel 8代i5 + nvidia gtx1050ti

### 安装python和git

注意要把python和git都添加到环境变量中，其次python版本最好是3.10系列

### 克隆webui仓库

```bash
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git
```

### 编辑bat自动化脚本

修改webui-user.bat文件

```bash
@echo off

set PYTHON=D:\Programs\Python\Python310\python.exe # 此处填写你的python路径，注意不能有中文和空格
set GIT=
set VENV_DIR=lightmon # 此处为nenv路径，可随意填写
set COMMANDLINE_ARGS=--lowvram --deepdanbooru --xformers # 此处为启动参数，我的gtx1050ti显存太小，因此启用这些参数，因为是gtx1000系显卡，因此可以自动安装xformers

call webui.bat
```

### 启动

双击bat文件自动开始安装所需环境，注意挂好梯子

### 其他

启动web界面可能会有error-expected char巴拉巴拉的，这个把代理关掉刷线就好了

### 模型

模型获取网站

https://civitai.com/

https://huggingface.co/

推荐模型：



### 插件

https://github.com/DominikDoom/a1111-sd-webui-tagcomplete

https://github.com/kohya-ss/sd-webui-additional-networks

https://github.com/Mikubill/sd-webui-controlnet


