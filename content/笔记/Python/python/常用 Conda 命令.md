##### 常用 Conda 命令
```shell
python
# 进入当前环境的python解释器，默认base环境

conda create --name [yourEnv] python=[version]
# 创建环境
# conda create --name data python=3.8

conda env remove --name [yourEnv]
# 移除环境
# conda env remove --name data

conda info -e
conda env list
# 环境列表

conda env export > environment.yml  
# 复制环境信息为yaml

conda env create -f environment.yml  
# 从yaml重建环境

conda config --show-sources
# 镜像源

conda config --add channels
# 添加镜像源
# conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
# conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
# conda config –-add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/free/
# conda config --add channels http://mirrors.aliyun.com/pypi/simple/

conda activate 
# 激活切换环境
# conda activate env-name

conda deactivate
# 退出当前环境

conda list
# 包列表

conda install
conda install --file
# 安装包
# conda install numpy
# conda install pandas
```
