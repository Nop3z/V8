FROM ubuntu:20.04
ENV LANG C.UTF-8
ENV DEBIAN_FRONTEND noninteractive
RUN sed -i 's@http://archive.ubuntu.com/ubuntu/@http://mirrors.aliyun.com/ubuntu/@g' /etc/apt/sources.list

RUN apt-get update -qq # apt-get update && install operation
RUN mkdir -p /root/directory
WORKDIR /home/nop/dokcer/v8
RUN     apt-get clean && \
    apt-get update && \
    apt-get install -y python3 python3-dev python3-pip build-essential
#以上操作apt-get 清理缓存, update ,安装python3.8以及安装python模块 的一系列操作
RUN apt-get install -y wget curl vim git sudo I# apt-get 安装wget curl vim
ENTRYPOINT [ "/bin/bash" ] #执行shell脚本