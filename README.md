---

# 联系方式

- 手机：18642636963
- Email：fuhuixiang@jonnyf.com
- QQ/微信号：644612679

---

# 个人信息

 - 付会翔/男/1991 
 - 本科/大连民族大学计算机科学与技术 
 - 工作年限：3年
 - 技术博客：http://www.cnblogs.com/fuhuixiang
 - Github：https://github.com/F-happy
 - 期望职位：Web前端开发工程师
 - 现居城市：北京

---

# 工作经历

## 北京便利蜂商贸有限公司（ 2017年10月 ~ 至今 ）

### 蜂掌柜订货系统
> 技术栈 react-native + redux + redux-observable + rxjs

这个项目是便利店中负责店长每天订货的系统，运行在 android 平板上，可以方便的为店员提供每日的商品订货功能、销售数据查询、销售报表统计等功能。

这个项目中我负责订货页面中核心的操作交互部分，以及商品分类的展示表格。这个项目的难点在于对于react-native中View节点过多导致的渲染卡顿，后来我通过减少view节点+最小化渲染范围+优化官版ListView组件来减少用户在操作中的卡顿感。

### 语音点餐应用
> 技术栈 react-native + redux + redux-observable + rxjs + flow

这个项目是便利店中热餐售卖区域中方便店员快速下单承单的应用。在用户选取热餐的时候店员可以通过语音指令的方式或者手动点击屏幕上的商品来添加购物车，在通过扫描用户的人像将订单与用户绑定，在用户去自助POS结账时自动与用户的订单绑定，完成热餐的购买。

这个项目中我一个人完成整个应用的开发，这个项目的难点在于通过底层调用百度的语音服务来完成对用户信息的解析（音频+视频），由于这个项目涉及的其它服务众多，对于链接这些服务设备的枢纽和与用户交互的前端，需要对各个数据源的数据进行整合、处理、容错等消费行为。

### 门店设备监控平台
> 技术栈 nodejs + Koa2 + kafka-node + redis + MySQL

这个项目是一个nodejs的后端服务，主要用于解决门店中众多设备的异常报警、设备在线等问题。在这个项目中提供了自动轮询设备在线状态、设备报警的消息（内部通讯软件+短信+电话）通知、以及一些公共功能的服务。其中通过对设备上报上来的日志频率以及日志中有可能包含的异常信息来发送kafka消息给公司内部消息对列触发报警+升级逻辑。

我在这个项目中开发了大多数的功能和代码。以及开发后台管理页面等页面。

### 门店收银POS
> 技术栈 react-native + redux-observable + rxjs + redux

这个项目包含销售报表的查询与显示、历史订单的查询与显示、店员的现金收银+用户自助的在线支付的收银台、挂账、无小票退货、现金回收、充值中心等功能。其中最重要的就是收银台模块，用户可通过自助POS机来下单结账，最大程度的减少用户在人工台排队等候的时间。

这个项目为了简化前端对于数据的处理压力，在前端app与后端服务中增加了一层offline client服务，由APP发出的所有接口都会被拦截，并通过进程间的通讯从离线客户端中获取数据，从而在第一次初始化后对于商品信息的加载就会非常的快。另外我们的扫描枪可以通过扫描包含收款码在内的各种二维码、条形码来快速的编辑购物车或者为用户提供结账功能。还有对于小票的打印我们也在前端处理，通过调用小票打印机提供的SDK服务来打印我们想要的格式和内容，并且在业务层面我们通过封装类似JSX的语法来方便业务打印小票内容。

### 无人店进出门
> 技术栈 react-native + redux

我们除了正常的便利店外还有集装箱式的无人店，其中在无人店中的进出门也是由前端通过rn来控制的。当用户扫描或者人脸识别确认身份后无人店的门就会打开，让用户进入无人店中购买东西，在无人店中的商品都贴有RFID标签，当用户携带商品走到门口时，感应器通过扫描到的RFID商品自动为改用户承单。在用户完成订单支付后会重新打开无人店的门让用户离开。

这个项目还处于试验阶段，还存在很多问题，但主流程已经稳定，并且在实际中也有投放使用。

## 上海喔噻科技股份有限公司（ 2017年3月 ~ 2017年9月 ）

### CRM项目客户端
> 技术栈 react + react-native + redux（后期改造成 mobx）

整个app基于react-native开发，我负责主要框架的搭建和大部分的日常开发工作，主要功能包括新增商户的整个入网流程的各个生命周期的跟踪和修改，例如入网、资料提交、资格审核、驳回修改等。还有线下BD人员数据的统计展示。以及一些商户管理、维护等功能。

### CRM项目中间层
> 技术栈 node + Koa2 + GraphQL

由于后期功能变多，版本迭代加快，之前的java维护的api层开发效率逐渐跟不上了，并且web页面和客户端页面中大量需要请求多个api才能完整的拼接出页面所需内容，并且两端内容显示差异明显，因此冗余的网络请求次数和返回结果影响了整体的用户体验。所以在客户端和底层数据间加入一层中间层用来聚合数据，并通过GraphQL的优势来去除冗余的数据和请求。

## 广州优蜜科技 （ 2015年7月 ~ 2016年5月 ）

### 零钱夺宝项目
> 技术栈 react + react-router + scss + webpack

我在这个项目中作为前端主程，开发了 web 版本的项目（ReactJS），在这个项目中我从零开始搭建了全部的前端架构，完成了从 web 版本的开发到测试到发布的全部流程。比较难处理的地方是在商品开奖的倒计时，有时等待开奖的商品特别的多，所以采用传统 setTimeout 会直接卡死页面，所以通过队列的形式同时对多组相同时间的倒计时进行合并计算。这个项目从我加入时的日流水几千到我离开项目组时日流水过500万，整体来说还算一个比较成功的项目。

### 宣传活动页
> 技术栈 JavaScript(ES6) + scss + html + nuts

在开发夺宝项目的同时，我还带着实习生在做客户端中的各种活动页面，保证逢年过节有大活动，不定时有小活动热身的节奏。除平日里做活动页之外，为了减轻同事开发时非逻辑需求的打扰，我在 gulp4 的基础上开发了前端工程构建工具(类似 fis3) [NUTS](https://github.com/F-happy/nuts)，从而解放了同事的生产力，面对大量的活动，仅仅只需要每次执行几个命令就可以自动的创建模板代码，创建本地开发环境，自动进行代码编译和发布。

## 深圳快箭科技 （ 2016年3月 ~ 2017年2月 ）

### 许愿夺宝活动 
> 技术栈 js + scss + html + nuts

在有米后期离职出来和同事创立快箭公司，更名许愿夺宝后继续运营。这个时候由我一个人维持之前项目的前端部分。

### 虚拟卡项目 
> 技术栈 react(全家桶) + ant-design(UI) + scss + webpack

在公司后期转型后主做京东卡转卖业务，这个时候我和后端采用前后端分离的方式开发提供卡商使用的各种后台系统。项目分移动端和 PC 端，UI 采用的 ant-design，移动端是兼容 react-native 的代码，可以很快的编译出 ios 和 Android 的应用(最终没有实现)。

### 其他项目

公司内部的各种系统后台，均是前后端分离，前端部分都使用 React 全家桶来进行开发，UI界面均采用[Ant Design](https://ant.design/docs/react/introduce-cn)。

---

# 开源项目和作品

## 开源项目

 - [NUTS](https://github.com/F-happy/nuts)：基于 gulp#4.x 的前端工程构建集合，包括了最常见的新建项目，开发项目和最后的编译发布项目。![npm](https://img.shields.io/npm/dt/wishbao.svg?style=flat)

 - [nuts-scss](https://github.com/F-happy/nuts-scss)：一个 scss 的基础样式库， 一个基于 node-sass 的 “compass”。

 - [gulp-replace-pro](https://github.com/F-happy/gulp-replace-pro)：一个加强版的 gulp-replace 插件。

- [verification-code](https://github.com/F-happy/verification-code)：前端随机生成验证码的小工具, 利用了前端中的 canvas 画布来进行数字的展示。

- [nuts-desktop](https://github.com/F-happy/nuts-desktop)：一个支持全平台的图像界面版前端工具流。

- [mobile-rotate](https://github.com/F-happy/mobile-wheel-of-fortunep)：这是一个由原生 js 编写的移动端高性能转盘插件。


## 技术文章
> [博客园地址](http://www.cnblogs.com/fuhuixiang/)，忙的很久没更新了...

- [我的前端故事--高仿支付宝密码输入框](http://www.cnblogs.com/fuhuixiang/p/5083660.html)
- [我的前端故事----优美的编辑器GitHub Atom](http://www.cnblogs.com/fuhuixiang/p/4840866.html)
- [端页面--天猫右侧信息栏弹出效果实现](http://www.cnblogs.com/fuhuixiang/p/4342607.html)
- [我的前端故事--疯狂倒计时(requestAnimationFrame)](http://www.cnblogs.com/fuhuixiang/p/4957802.html) 


# 技能清单

以下均为我熟练使用的技能

- Web开发：Node
- Web框架：Koa2/GraphQL
- 前端框架：React/React-native
- 前端工具：Gulp/SASS/Grunt/Webpack
- 版本管理工具：Git
- 云和开放平台：微信小程序

---

# 致谢
感谢您花时间阅读我的简历，期待能有机会和您共事。

