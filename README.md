# hao

> A simple navigation site project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


## Build docker image

```bash
# build a simple docker image from nginx
docker build -t hao .

# run a container 
docker run \
--name hao \
-p 80:80 \
-v /home/alex/workspace/nodejs-hao/hao.conf:/etc/nginx/conf.d/default.conf:ro \
-d --restart=always \
hao:latest
```
