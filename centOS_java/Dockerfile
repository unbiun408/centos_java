# 使用 CentOS 作为基础镜像
FROM centos:7

# 设置工作目录
WORKDIR /app

# 安装必要的软件包并安装 OpenJDK
RUN yum -y update && \
    yum -y install java-1.8.0-openjdk-devel && \
    yum clean all

# 验证 Java 安装
RUN java -version

# 设置容器启动时的默认命令
CMD ["java", "-version"]
