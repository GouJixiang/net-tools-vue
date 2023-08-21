# OCCN Admin

基于 `Vue3 + Vite + TypeScript + Naive UI` 打造的网络资产管理平台🌏

## 一、运行项目及编译打包
项目使用 **yarn** 作为包管理器，如需启动项目，要先安装yarn。yarn安装命令：
```shell
npm i -g yarn
```
###  1.1 YARN方式启动及编译打包
在项目根目录下按顺序执行下面的命令即可启动：
```shell
yarn install
yarn run dev
```
如需打包，执行下面的命令：
```shell
yarn build
```
### 1.2 Docker操作
在安装了Docker的前提下，在项目根目录执行：
```shell
# 打包镜像
docker build -f ./docker/Dockerfile -t net-tools-vue:v0.1 .
# 启动打包好的镜像
docker run -itd -p 80:80 net-tools-vue:v0.1
```
访问地址：http://127.0.0.1/

注：v0.1代表镜像的标签（版本），可根据实际需要修改
