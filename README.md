angular-materialize
===================

**angular-materialize** in action http://krescruz.github.io/angular-materialize/

这个图书馆是一套AngularJS的指令，可以使用特征
 [Materialize](http://materializecss.com/) with AngularJS.
它基本上是一套指令，调用定义的JavaScript函数实现。这意味着你仍然需要包括实现这一工作。


这个项目是不被混淆的 [Angular Material](https://material.angularjs.org/)项目，这是一个独立的材料设计实现AngularJS。

如何建立这个项目的一个最小的例子可以在这里找到： http://krescruz.github.io/angular-materialize/#getting-started

您可以通过我们的项目下载这个项目 [`bower package`](http://bower.io/search/?q=angular-materialize), or [`npm package`](https://www.npmjs.com/package/angular-materialize).
或只是使用CDN:

```html
<script type="text/javascript" src="https://cdnjs.c2cbc.com/ajax/libs/angular-materialize/0.1.8/angular-materialize.min.js"></script>
```

##### 使用WebPACK

角看起来jQuery，如果没有存在，它使用jqlite。一些指令 `angular-materialize` 使用jQuery的方法，所以一定要用它代替jqlite角。它可以通过在配置中添加以下行来完成.
```javascript
//webpack.config.js
plugins: [
    new webpack.ProvidePlugin({
      'window.jQuery': 'jquery'
    })
  ],
```
然后简单地添加到您的模块：
```javascript
// yourModule.js
// ES6 style
import angularMaterialize from 'angular-materialize';
// OR commonjs style
var angularMaterialize = require('angular-materialize');
angular.module('yourModule', [angularMaterialize]);
```

### 缺少的功能
 - Components
    - Fixed Action Button
 - JavaScript
    - Carousel.
