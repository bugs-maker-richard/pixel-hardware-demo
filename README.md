# PIXEL / LAB · 像素硬件

J1900 小主机与树莓派 5 的静态购物流程演示。

网站：https://bugs-maker-richard.github.io/pixel-hardware-demo/

打开 index.html 即可浏览。GitHub Pages 使用 main 分支根目录发布。

功能：首页、商品列表、独立详情、实拍图切换、购物袋和数量调整、模拟付款与完成页、联系表单。

**本项目不收款、不产生真实订单、不发货。** 199 元和 399 元均为虚构演示价格。
联系表单仅验证邮箱和问题并显示预览，未配置邮件或收件后端，内容不会发送。
树莓派原始文字描述写 1GB，但图片包装写 8GB，已在页面标注版本待确认；照片中的配件不代表包含。

修改商品信息与演示价格：app.js 的 PRODUCTS。样式：styles.css。图片：assets/。
浏览器 localStorage 仅用于保存购物袋，不存储邮箱或问题。

基于 MIT 开源项目 [Start Bootstrap Shop Homepage](https://github.com/StartBootstrap/startbootstrap-shop-homepage) 的 Bootstrap 样式基础定制。原许可见 vendor/LICENSE-startbootstrap.txt，Bootstrap 许可亦保留于样式文件头部。
静态资源均存储于仓库，无 CDN 依赖。

