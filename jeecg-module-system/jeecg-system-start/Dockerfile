FROM  openjdk:8-jre
# author
MAINTAINER xingyun.xie@huamod.com
RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
WORKDIR /jeecg-boot
EXPOSE 2101
ADD ./target/jeecg-system-start-3.6.2.jar ./
# 启动认证服务
ENTRYPOINT ["java","-jar","-Dserver.port=9103","-Dspring.profiles.active=test","jeecg-system-start-3.6.2.jar"]