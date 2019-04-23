FROM registry.cn-hangzhou.aliyuncs.com/wtx/node-nginx:latest
COPY . /app/
RUN cd /app/server
RUN npm config set sass-binary-site http://npm.taobao.org/mirrors/node-sass
RUN npm install && npm start
EXPOSE 7001

