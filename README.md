<<<<<<< HEAD
# 时间控件

#### 介绍
{**以下是码云平台说明，您可以替换此简介**
码云是开源中国推出的基于 Git 的代码托管平台（同时支持 SVN）。专为开发者提供稳定、高效、安全的云端软件开发协作平台
无论是个人、团队、或是企业，都能够用码云实现代码托管、项目管理、协作开发。企业项目请看 [https://gitee.com/enterprises](https://gitee.com/enterprises)}

#### 软件架构
软件架构说明


#### 安装教程

1. xxxx
2. xxxx
3. xxxx

#### 使用说明

1. xxxx
2. xxxx
3. xxxx

#### 参与贡献

1. Fork 本仓库
2. 新建 Feat_xxx 分支
3. 提交代码
4. 新建 Pull Request


#### 码云特技

1. 使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2. 码云官方博客 [blog.gitee.com](https://blog.gitee.com)
3. 你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解码云上的优秀开源项目
4. [GVP](https://gitee.com/gvp) 全称是码云最有价值开源项目，是码云综合评定出的优秀开源项目
5. 码云官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6. 码云封面人物是一档用来展示码云会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
=======
# vue-date-time-m


移动端好用的时间日历组件没有找到合适的，遂自己写了个。
UI部分借鉴了  [vue-persian-datetime-picker](https://talkhabi.github.io/vue-persian-datetime-picker) 真的做的很棒，可惜是阿拉伯的日期显示方式


### 图例

![](https://github.com/mayufo/vue-date-time-m/blob/master/img.gif)

### 在线demo
[demo](https://mayufo.github.io/vue-date-time-m/)

### 更新

#### 1.0.27
 1. 增加了时间的间隔，详情可见demo
 2. 可以选择年月日时，而不选择分钟

### npm

```
npm install vue-date-time-m
```

### use
- main.js

```
import dateTime from 'vue-date-time-m';
Vue.component('data-time', dateTime);
```

- in component
```
        <template>
          <div class="date-time-item">
            <div class="date-time-input" @click="show">{{ data }}</div>
            <d-date-time ref="dateTime"
                         type="date"
                         @confirm="select"></d-date-time>
          </div>
        </template>

        <script>
          import DateTime from 'vue-date-time-m'
          export default {
            data(){
              return {
                data: ''
              }
            },
            components: {
              DateTime
            },
            methods: {
              //  展示日期组件
              show () {
                this.$refs.dateTime.show()
              },
              // 日期组件回调
              select (val) {
                this.data = val
              }
            }
          }
        </script>
```
>>>>>>> 时间
