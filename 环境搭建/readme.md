# 构建容器
`sudo docker build -t v8 .`
# 运行容器
`sudo docker run -it --entrypoint /bin/bash v8`
# 下载依赖
## 下载ninja
`git clone https://github.com/ninja-build/ninja.git`
`cd ninja && ./configure.py --bootstrap && cd ..`
echo `export PATH=$PATH:"/home/ninja"` >> ~/.bashrc
`source ~/.bashrc`
## 其他依赖
`sudo apt install bison cdbs curl flex g++ python vim pkg-config`
`git clone https://chromium.googlesource.com/chromium/tools/depot_tools.git `