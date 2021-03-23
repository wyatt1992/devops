
# 拉取Python3 镜像作为基础镜像
FROM rackspacedot/python37

# 将工作目录切换为/app
WORKDIR /app

# 将当前目录下的所有内容复制到/app下
ADD . /app

# 使用pip命令安装这个应用所需要的依赖
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# 允许外界访问容器的18080端口
EXPOSE 18080

# 设置容器进程为：python app.py，即：这个Python应用的启动命令
CMD ["python", "app.py"]