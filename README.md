# taobaoVisitingVenues

## 简介

**618快乐呀**

现在开始支持淘宝和京东的自动浏览任务了。解放双手不用手动点击，自动就能浏览，类似按键精灵的操作。

本脚本基于 Auto.js Pro 7.0 开发。官网 [Auto.js](https://pro.autojs.org/  "Auto.js") （现在为 Pro 8.0），该作者 [hyb1996](https://github.com/hyb1996) 的开源项目地址为 [Auto.js](https://github.com/hyb1996/Auto.js) 。

如果嫌 [GitHub](https://github.com/sleepybear1113/taobaoVisitingVenues) 下载速度慢，可以去 [Gitee](https://gitee.com/sleepybear1113/taobaoVisitingVenues) 下载 apk。Gitee 的主要的内容都是同步这里的。

## 目前已知问题

1. 存在悬浮窗权限导致初次启动失败的问题。
2. 逛店到最后可能会回到首页。然后可能无法返回领取中心了。
3. 其他隐藏的诸多问题。

## 最新更新日志

### 05/23 11:30 【京东 - floating -> 3, script -> 2】

1. 再次修复无法二次启动/开始

## 其他

1. 系统需要 Android 7.0 及以上
2. 第一次开启APP授予权限即可【电话权限可能不是必需，储存权限必须(联网下载脚本)】
3. 由于 auto.js 的工具显示对话框需要悬浮窗权限，所以点击按钮前需要授权悬浮窗权限。
4. 每逢 APP 级别的更新或者安装，执行清除本地脚本
5. 在主界面右上角三点，点开有查看日志的选项
6. 无障碍开启方法:点击悬浮窗启动后转到无障碍设置界面，选择该 APP 开启。某些手机可能因为悬浮球或者全面屏手势而显示遮挡无法开启。

## 部署问题

### 工具

auto.js pro 7.0.4。现在能看见的只有 free 版的 auto.js 4.0 和收费版的 auto.js pro 8.0。没有 pro 7.0 了。

7.0 和 8.0 的区别就是，8.0 对灰产行业进行了一定的限制，所以对淘宝在内的一些 APP 进行了屏蔽，代码可能在 8.0 上面无法正常运行。

不过也许可以在 free 的 4.0 版部署（不过我没有试过，毕竟我有 pro 7.0 的账号）。

关于 free 版的 auto.js，是个开源项目，参见这个仓库 [Auto.js]: https://github.com/hyb1996/Auto.js ，里面有相关的使用。

### 主要步骤

将`src`里面的代码全部下载，放置于`手机储存/脚本/淘宝京东`目录，将全部的文件移到里面，刷新 auto.js 就能看到新的项目了。

#### 目录结构

`update`文件夹内为更新新脚本的辅助类工具文件，`main.js`为入口类脚本，启动`UI.js`来展示界面。

#### 更新脚本

更新脚本的地址使用了国内的 Gitee 以提升使用体验。下载的脚本放置于`手机储存/脚本/Internet/淘宝京东/`下，根据不同脚本名建立了文件夹。

# 更新日志

## 2.0 新版脚本更新记录

### 05/21 23:30 【京东 - 悬浮窗 floating 更新 version 2】

1. （修复）二次启动可能报错。

### 05/21 23:30 【app/脚本 全面更新 version 2.0.0】

1. （发布）新版apk 2.0.0，更加人性化了一些（存在悬浮窗权限导致初次启动失败的问题）。
2. （更新）京东脚本初版。能解决部分自动化问题，但是还是存在点击后回到首页的问题。同时那些点击会跳转首页的以列为一个列表暂不点击（列表不完全）。
3. 将旧淘宝脚本也转移了过来。
4. 新脚本发布，问题多多，请包涵（可能限于毕设进度推迟更新）。
5. `src`文件全面更新，旧版`src_code`不再使用。

## 1.0 旧版脚本更新记录

----------------------------2020----------------------------------

### 1.1.8 01/03 20:00 【脚本在线更新】

1. （改）优化时间控制 A.避免了可能存在的少 1 秒的情况。 B.更加契合本次的活动的流程。

----------------------------2019----------------------------------

### 1.1.7 12/02 14:35 【脚本在线更新】

1. （增）新增去搜索的浏览过程。
2. （改）优化时间控制，浏览次数满了之后快速返回刷新。

### 1.1.6 12/01 11:00 【脚本在线更新】

1. （改）双 12 更新第一弹，更新双十一脚本为双 12 脚本。

### 1.1.5 11/10 10:20 【脚本在线更新】

1. （改）修复点击“领喵币”打开盖楼结束的提示页面

### 1.1.4 11/05 23:20 【脚本在线更新】

1. （改）较大程度解决浏览店铺出现 5s 广告，进行跳过。5s 广告出现次数很少虽然不影响正常操作，但是还是进行了跳过。

### 1.1.3 11/04 18:45 【脚本在线更新】

1. （改）修复“猜你喜欢”出现同时逛店消失但次数没满，直接去首页的情况（此时可能会增加几次开闭领取中心的次数）

### 1.1.2 11/03 09:50 【脚本在线更新】

1. （改）优化浏览时间的控制，将浏览时间控制在 30s 内（一般在 20s 内），防止手机息屏

### 1.1.1 11/01 22:45 【脚本在线更新】

1. （增）运行中toast提示，增加友好性
2. （增/测试）浏览店铺顺便签到领币（开启方式：“功能选择”中选择第二个）

### 1.1.0 11/01 19:30 【apk 发布】

1. （改）将更新地址改为 Gitee 的 raw。因为 GitHub 的 raw 经常不能访问。
2. （新）解决淘宝浏览某个会场后，返回的时候需要两次
3. （改）每运行 5 次就重新关闭“领取中心”并重新打开
4. （改）将旧代码改得好一些了
5. （重要）需要将本地脚本清除！！！！！！！！
6. （删）将选择功能的选项砍了，虽然悬浮窗的还在，但其实已经没有作用了

### 1.0.6

1. 将去首页浏览猜你喜欢暂时不点击直到全部浏览结束
2. 初版脚本，具体更新情况我也忘记了
