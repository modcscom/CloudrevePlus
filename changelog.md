## CloudrevePlus/更新日志
### 后端
+ routers/controllers/admin.go
  - :27 禁用获取社区新闻功能
+ routers/router.go
  - :404 删除社区新闻相关路由
  - :387 举报接口增加验证
+ middleware/frontend.go
  - :51 解决无法获取站点描述问题
+ models/defaults.go
  - :18 更改默认站点描述为'部署公私兼备的网盘系统'(选自官网)
  - :109 更改默认文件样式为'列表'
  - :108 添加设置'允许举报分享'(默认关闭)
+ pkg/conf/version.go
  - :4 为与正式版作区分增加'Plus版本号'

### 前端
+ src/config.ts
  - :20 修复字幕文件后缀'vtt'写成'vrr'的问题
  - :any 添加更多可在浏览器中预览的文件类型
+ src/component/Viewer/PDF.js
  - :13 更换pdf.js CDN地址为staticfile
+ src/component/Admin/Index.js
  - :172 删除请求社区文章部分
+ src/component/FileManager/MusicPlayer.js
  - :any 优化控制逻辑，允许调节音量

### 其它
+ 允许举报分享
  - 举报功能没有限制，可能会被恶意利用刷数据库
  - 可在后台→参数设置→增值服务中找到相关设置
