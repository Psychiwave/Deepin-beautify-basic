*教程请参考：*

在这基础上由于个人需求定制了一套自己的配置，具体的教程搜索引擎上都有，但是为了方便自己检索于是有了本条记录：

## 字体

   * 先打开权限`chmod -R 777 /usr/share/icons/`然后进入 `cd /usr/share/icons/` 右键"在文件夹中打开"然后把`fonts`里的文件都拖过去(包含windows字体)，最后把权限改回来`chmod -R 755 /usr/share/icons/`然后进入 `cd /usr/share/icons/`
## 图标
  * 同上，把路径改为`icons` 
    ## 窗口主题
  * 同上，把路径改为`themes`
    ## 桌面壁纸（&自动更换）
  * 在`~/.config/autostart`下将`changewallpaper.desktop`文件放入
    参考：[撸了一段自动更换壁纸的脚本](https://bbs.deepin.org/forum.php?mod=viewthread&tid=38940)

## 桌面图标更改

* **mac图标**：https://github.com/keeferrourke/la-capitaine-icon-theme

## 主题音效更改

* 1.Win+E 打开文件管理器  进入到目录：`/usr/share/sounds/deepin/stereo`
* 2.右键管理员打开当前文件夹  把(例：`钉宫语音包.tar.gz`）解压后的语音包 全部替换

参考：[【死宅限定钉宫语音包】](https://bbs.deepin.org/forum.php?mod=viewthread&tid=154264)和[elementaryOS音效](https://bbs.deepin.org/forum.php?mod=viewthread&tid=134778)

## grub背景更改

**grub背景图片目录**
 `/boot/grub/themes/deepin/background.jpg`

去除默认选项框：
修改 `/boot/grub/themes/deepin/theme.txt`
将 `menu_pixmap_style = "menu_*.png"`
用 `#`注释掉即可

**注：如果只是更换壁纸的话，打开`设置`>`控制中心`（最下面）>`启动菜单`，直接把想更换的壁纸拖进去即可，还可以设置是否开启主题和启动延时**

## 插件安装   

 * **conky桌面插件**
   * **.conky**：解压`shuxun2.tar.gz`，将`.shuxun2`放入`/home/.conky/`中（Ctrl+H 显示隐藏文件）

   * **conky manager**：deepin商店搜索下载，选中`.shuxun`,然后在设置里设置开机启动

## 音频优化

`sudo apt install jackd pulseaudio-module-jack caps`

详细教程：[简单一步 大幅提升linux音质 耳返设置方式](https://www.bilibili.com/video/av43862110)

