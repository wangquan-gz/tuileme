# 你推了么 - 纯前端静态版

## 功能特性
- ✅ 完全离线可用，数据存在浏览器本地（IndexedDB）
- ✅ 项目卡片：黄色进行中、绿色已完结
- ✅ 进度记录：自动记录时间，最新在最上方
- ✅ 长按菜单：修改、删除
- ✅ 导出Excel：多选、全选，自动带日期文件名
- ✅ 导出后自动清理已完结项目
- ✅ 完结/取消完结功能，项目位置不变
- ✅ 严格按创建时间排序，最新创建在最顶端
- ✅ PWA支持，可安装到手机桌面
- ✅ 移动端适配，操作流畅

## 文件说明
- index.html - 主程序（所有功能都在这一个文件里）
- manifest.json - PWA应用清单
- sw.js - Service Worker 离线缓存
- app-icon.png - 应用图标

## 部署方法

### Vercel 部署（推荐，免费最简单）
1. 解压zip文件
2. 打开 vercel.com 登录
3. 点击 Add New → Project
4. 选择 Upload，上传整个解压后的文件夹
5. 直接点 Deploy，等待1分钟完成

### 其他平台
- Netlify - 同样支持拖拽上传
- GitHub Pages - 上传到GitHub仓库
- 腾讯云COS / 阿里云OSS - 对象存储静态网站
- 自己的服务器 - 放到Nginx/Apache静态目录

## 手机安装PWA
部署到HTTPS网站后：
1. 手机Chrome浏览器打开网址
2. 等页面完全加载
3. 右上角菜单 → 安装应用
4. 桌面出现图标，全屏运行，完全离线可用

## 打包APK
部署后可以用在线工具打包：
- webintoapp.com - 最简单，填网址直接生成
- pwabuilder.com - 微软官方PWA打包工具
- appsgeyser.com - 另一个选择

## 数据说明
- 所有数据存在浏览器本地IndexedDB
- 清除浏览器数据或卸载PWA会丢失数据
- 建议定期导出Excel备份
