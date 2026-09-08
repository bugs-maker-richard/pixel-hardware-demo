# PIXEL / LAB · 像素硬件课程作业

J1900 小主机与树莓派 5 的静态购物网站。

网站：https://bugs-maker-richard.github.io/pixel-hardware-demo/

打开 index.html 即可浏览。GitHub Pages 使用 main 分支根目录发布。

功能：首页、商品列表、独立详情、实拍图切换、购物袋和数量调整、中英文切换、首次访问用户协议确认、Cookie 授权与偏好窗口、Stripe 风格付款窗口、联系表单。

付款最后一步是本地构建的 Stripe 风格界面，不加载 Stripe SDK，也不连接任何支付接口。
流程：确认购物袋 → 进入付款窗口 → 点击支付 → 显示“付款功能正在开发中，敬请期待”。
付款窗口中的邮箱与卡片内容是固定展示文本，不可编辑、不会收集或发送。
首次打开网站时会显示十三条中英文用户协议预览框，点击“同意并继续”后才能进入网站；接受状态只保留在当前页面，刷新后会再次出现。结算页会同步勾选协议。
页面右上角提供中英文切换按钮，首次用户协议弹窗内也可切换语言。语言选择保存在浏览器本地存储中。
Cookie 授权仅改变当前页面状态，不设置统计或广告 Cookie，也不向第三方发送选择记录。刷新页面后授权条会再次出现。
联系表单仅验证邮箱和问题并显示预览，未配置邮件或收件后端，内容不会发送。
树莓派原始文字描述写 1GB，但图片包装写 8GB，已在页面标注版本待确认；照片中的配件不代表包含。

修改商品信息与价格：app.js 的 PRODUCTS。样式：styles.css。图片：assets/。
浏览器 localStorage 仅用于保存购物袋，不存储邮箱或问题。

基于 MIT 开源项目 [Start Bootstrap Shop Homepage](https://github.com/StartBootstrap/startbootstrap-shop-homepage) 的 Bootstrap 样式基础定制。原许可见 vendor/LICENSE-startbootstrap.txt，Bootstrap 许可亦保留于样式文件头部。
静态资源均存储于仓库，无 CDN 依赖。

