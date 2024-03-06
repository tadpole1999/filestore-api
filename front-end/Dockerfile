# 使用官方的 nginx 映像作為基礎映像
FROM nginx:latest

# 將 Flutter build 的內容複製到 Nginx 的默認目錄
COPY web/ /usr/share/nginx/html/

# 使容器聽80端口（你可以選擇其他端口，但需要相應地更新 Nginx 配置）
EXPOSE 80

# 使用自訂的 Nginx 配置（可選，如果你需要自訂配置的話）
# COPY custom-nginx.conf /etc/nginx/conf.d/default.conf

CMD ["nginx", "-g", "daemon off;"]
