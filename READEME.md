### 使用步骤
#### 1、项目存放目录

直接把对应项目git拉下来放到packages文件夹下面
#### 2、设置依赖配置
在package.json里面更改workspaces，例子："packages/[项目名称]",

#### 3、使用方法
跟目录跑 yarn  

### 安装组件（单项目）
#### packageA 安装 axios
yarn workspace packageA add axios

#### packageA 移除 axios
yarn workspace packageA remove axios

### 安装组件（全部项目，慎用）
#### root package 安装 commitizen
yarn add -W -D commitizen

#### root package 移除 commitizen
yarn remove -W commitizen


### 运行单个 package 的scripts 命令
yarn workspace packageA dev


### 打包
yarn workspaces run build


