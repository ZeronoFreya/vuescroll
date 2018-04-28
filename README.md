
 
  <p align="center"><a href=""><img width="100" src="https://github.com/wangyi7099/pictureCdn/blob/master/allPic/others/logo.png?raw=true" /></a></p>

  [中文README](https://github.com/wangyi7099/vuescroll/blob/dev/README-ZH.md)<br />
  **Vuescroll** is a virtual scrollbar based on [vue.js 2.X](https://github.com/vuejs/vue) ，and it  has multi  modes you can choose, such as **slide** mode, **native** mode,  and **pure-native** mode. It also supports customizing styles of scrollbar，detecting size change of content、paging、pull-refresh，push-load and so on.

  <a href="https://www.npmjs.com/package/vuescroll"><img src="https://img.shields.io/npm/v/vuescroll.svg" alt="Version"></a><a href="https://circleci.com/gh/wangyi7099/vuescroll/tree/dev"><img src="https://img.shields.io/circleci/project/wangyi7099/vuescroll/dev.svg" alt="Build Status"></a><a href="https://www.npmjs.com/package/vuescroll"><img src="https://img.shields.io/npm/l/vuescroll.svg" alt="License"></a>
<a href="https://www.npmjs.com/package/vuescroll"><img src="https://img.shields.io/npm/dm/vuescroll.svg" alt="Download"></a>

## Features
* Has the basic behavior of the native scrollbar.
* Be able to customize styles of scrollbar(includes color, size, position, opacity, keep showing or not and so on).
* Switch among modes in runtime.
* Be able to smooth-scroll by setting the scroll animations, see [easing](https://wangyi7099.github.io/vuescrolljs/guide/Configuration.html#explanation-2).
* Support pull-refresh and push-load.
* Support paging(Slide a pull page each time).
* Support snapping(Slide a user-defined distance each time).
* Be able to detect the size change of the content.

## Demo
There are two ways to view demo:
1. Open the `demo` folder in the root of repo and go to view.
2. Go to online demo - [Offical Website](https://wangyi7099.github.io/vuescrolljs/guide/) to view.

## Get Started
### Install
### Install by npm or yarn
> Recommend yarn, why? Yarn will cache every modules you have installed, and won't download again next time when you use it.
```bash
npm install vuescroll -S
# yarn add vuescroll
```
### Usage
1. Configure in your entry file

```javascript
import Vue from 'vue' 
import vuescroll from 'vuescroll'

Vue.use(vuescroll)

const vm = new Vue({
    el: "#app",
    data: {
        ops: {
            vuescroll: {

            },
            scrollPanel: {
                
            }
            // ...
        }
    }
})
```
2. Wrap the content you want to scroll by vuescroll.
```html
<div id="app" >
    <vue-scroll :ops="ops">
        <div 
        class="content"
        v-for= "item in 100"
        :key="item"
        >
        <span>{{item}}</span>
        </div>
    </vue-scroll>
</div>
``` 

> For the detailed apis、events、configurations, please go to our [Offiacl Website](https://wangyi7099.github.io/vuescrolljs/).

## How to contribute

Firstly, thak you for you are interested in vuescroll!! Only follow some steps below to contribute code:
1. Fork this repo.
2. Clone the repo you have just forked.
```base
   git clone git@github.com:<Your Usernmae>/vuescroll.git
```
3. Modify the code in your local and push the code to your repo.
3. Click `New pull request` in vuescroll repo and that's all, like the picture below:<br /><img src="https://github.com/wangyi7099/pictureCdn/blob/master/allPic/others/pr.jpg?raw=true" /> 

## Inspired

[slimscroll](https://github.com/rochal/jQuery-slimScroll)    [element-ui](https://github.com/ElemeFE/element/tree/dev/packages/scrollbar/src) [scroller](https://github.com/pbakaus/scroller)

## License

**MIT** 

by wangyi7099