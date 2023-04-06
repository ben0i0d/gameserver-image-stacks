FROM openjdk:8-jre
RUN sed -i -E 's/http:\/\/(deb|security).debian.org/http:\/\/mirrors.tuna.tsinghua.edu.cn/g' /etc/apt/sources.list
RUN apt update && apt install -y locales
RUN echo "zh_CN.UTF-8 UTF-8">/etc/locale.gen && locale-gen
ENV LANG=zh_CN.UTF-8
ENV LANGUAGE=zh_CN.UTF-8
ENV LC_ALL=zh_CN.UTF-8
ENV TZ=Asia/Shanghai
RUN mkdir -p /workspace
WORKDIR /workspace
