# 基于官方Nginx alpine镜像（体积小、仅演示）
FROM nginx:alpine

# 将本地的index.html复制到容器内Nginx默认网站根目录
# 覆盖镜像自带的默认index.html
COPY index.html /usr/share/nginx/html/index.html

# 暴露80端口（Nginx默认监听端口）
EXPOSE 80

# 启动Nginx前台服务（保证容器不退出）
CMD ["nginx", "-g", "daemon off;"]
