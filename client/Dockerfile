FROM registry.cn-hangzhou.aliyuncs.com/wtx/node-nginx:latest
COPY . /app/
EXPOSE 80
RUN npm config set sass-binary-site http://npm.taobao.org/mirrors/node-sass
RUN npm install && npm run build  && cp -r dist/* /var/www/html
CMD ["nginx","-g","daemon off;"]

