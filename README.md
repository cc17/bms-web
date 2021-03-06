### 项目简介

积木(block)系统旨在为开发者、运营提供一套模块化开发、可视化页面搭建的解决方案。目的是尽可能的解放前端生产力，提高页面模块的复用率，并且充分赋予运营人员根据自身需要搭建、维护、发布页面的能力。

**bms-web**为积木系统的UI端项目，服务端(**bms-server**)项目尚未开放，并且，对于前端开发者进行页面模块开发的工具尚未开发完成，等后续开发完成以后会一并公开

### 特点

- 使用vue框架，告别琐碎操作dom的时代
- 使用ts框架，拥抱强类型时代
- 面向对象，面向接口编程，使得项目业务逻辑更清晰，扩展更好，维护更方便
- 加入依赖注入，使得功能依赖于接口，而不依赖于实现，扩展，维护更好
- webpack构建，紧跟前端模块化、组件化进程

### 项目结构简介

```
|-common 存放项目公用代码
|-components 存放项目公用组件
|-entry 各个页面的入口文件，webpack编译入口
|-interface 存放接口文件目录
|-models 存放业务实体目录
|-services 各个api接口服务
|-views 存放各个页面
```

### 运行项目

#### 安装依赖

```
npm/cnpm install
```

#### 修改bms-web项目某些地方

- 找到文件 **/src/scripts/views/design/index.html**，将html中的iframe标签的**src="/design/action"**修改为**/design.html**，否则页面搭建的模板读取的是部署到线上的模板，本地无法进行页面的搭建

#### 开发

```
npm run dev
```

#### 发布编译

```
npm run build
```
#### 运行build以后的项目

```
npm run serve
```
### 其他

- bms-web起来以后，本地看到的页面，数据即为线上的数据，因为api接口是代理到线上的
- 线上体验网站[积木系统](http://www.51qututu.com)
- 积木系统各页面简介，请[点击查看](https://github.com/ljcheibao/bms-web/blob/master/docs/introduce.md)
- 欢迎大家一起探讨跟指点，QQ:415026798

