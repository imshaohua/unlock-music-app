# unlock-music-app


## 介绍
 实际是 https://github.com/ix64/unlock-music 的Electron包装

## 支持格式
 QQ音乐 (.qmc0/.qmc2/.qmc3/.qmcflac/.qmcogg/.tkm)
 写入封面图片
 Moo音乐格式 (.bkcmp3/.bkcflac)
 QQ音乐Tm格式 (.tm0/.tm2/.tm3/.tm6)
 QQ音乐新格式 (实验性支持)
 .mflac
 .mgg
 网易云音乐格式 (.ncm)
 补全ncm的ID3/FlacMeta信息
 虾米音乐格式 (.xm) (测试阶段)
 酷我音乐格式 (.kwm) (测试阶段)
 酷狗音乐格式 (.kgm) (CLI版本)


## 使用说明
 使用mac的话,直接下载release的包,直接运行
 如果是windows的话,直接使用electron自行编译win版本

## 编译指南
 安装npm,如果速度太慢,那可以改用淘宝的镜像
 安装electron: sudo npm install electron -g
 安装packager: sudo npm install electron-packager -g
 试运行: npm run start
 自行打包命令: electron-packager . unlock-music-app --mac --out ./target --app-version 1.0.0 --electron-version=11.0.1 --overwrite --ignore=node_modules --icon ./favicon.ico

 --mac是输出mac执行文件, --win是输出win执行文件


 可以使用命令自己打包,也可以在下载的代码目录下:
    npm install
    npm run package (只打mac包)
