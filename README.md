## 什么是同源策略

- 协议相同
- 域名相同
- 端口号相同 

> 浏览器对cookie限制不可共享

> script form image iframe 不受同源策略限制

## cookie

只有符合同源策略的才能共享cookie，二级域名通过设置document.domain

## 如何设置同源策略（hosts）

> 最实用：后台设置 domain=xxx.com

## 利用img.src测网速

```javascript
const img = new Image();
const start = Date.now();
img.src = '/1.gif';
img.onload = function() {
  const end = Date.now();
  const v = (1k / (end - start)); // 伪代码
}
```

## 语义化

实用div布局  不用div包裹无意义的东西

尽量少写HTML