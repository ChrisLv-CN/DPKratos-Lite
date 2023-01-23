[![license](https://www.gnu.org/graphics/gplv3-or-later.png)](https://www.gnu.org/licenses/gpl-3.0.en.html)

关于Kratos-Lite（About Kratos-Lite）
============

原 `Kratos Build8` 现更名为 `Kratos-Lite`。   
The original `Kratos Build8` is now rename as `Kratos-Lite`.

新版本将深度结合DP2.1的框架结构，对代码进行完全重构，想比之前的版本，具有更轻量、更快的速度、更便捷的更新机制。   
The new version will deeply combine the framework structure of DP2.1, completely refactor the code, and have a lighter, faster and more convenient update mechanism than the previous version.

此仓库不包含源代码，仅保存非开发者Modder所需要的文件，需要查看源代码可前往[此处](https://github.com/ChrisLv-CN/DPKratos-Lite-Source)。   
This repository does not contain source code, it only saves files needed by non-developer Modders. If you need to view the source code, you can go [Here](https://github.com/ChrisLv-CN/DPKratos-Lite-Source).

关于Kratos (About Kratos)
============

DynamicPatcher是由开发者Xkein创建的尤里的复仇MOD开发平台，[项目主页](https://github.com/Xkein/YRDynamicPatcher)  
DynamicPatcher is Yuri's Revenge MOD *development platform* created by developer Xkein.

Kratos项目是尤里的复仇MOD《乱来时刻（WWSB HOUR）》的作者 **双杀步枪（ChrisLv_CN）** 所创建的DP应用项目。[MOD作者主页](https://space.bilibili.com/276838)  
Project Kratos is a DP application project created by **ChrisLv_CN**, the author of Yuri's revenge MOD "WWSB HOUR".

本项目完全基于DP进行开发，以INI标签的形式为MOD提供全新特性。  
This project is completely developed based on DP, and use INI labels to provides new features for MOD.

食用方法 (How to use)
------------

1. 前往[Release](https://github.com/ChrisLv-CN/DPKratos-Lite/releases)下载最新的压缩包。  
Go to [Release](https://github.com/ChrisLv-CN/DPKratos-Lite/releases) to download the latest package.

2. 把文件夹`DynamicPatcher`，文件`DynamicPatcher.dll`和`PatcherLoader.dll`放入尤里的复仇游戏根目录下。  
Put the folder `DynamicPatcher`, files `DynamicPatcher.dll` and `PatcherLoader.dll` into Yuri's Revenge game root directory.

3. 在`ini`中添加对应的内容。  
Edit `ini` file

4. 为`gamemd.exe`与`syringe.exe`添加管理员权限。（Build7起升级为DP2.0，不再需要设置管理员权限）  
Add administrator privileges to `gamemd.exe` and `syringe.exe`. (Build7 and later versions do not need this because update to DP2.0)

5. 运行`RunAres.bat`启动游戏。  
Run `RunAres.bat` to start the game.

帮助文档 (Documents)
------------
* [食用说明书](https://github.com/ChrisLv-CN/DPKratos-Lite/blob/main/DynamicPatcher/Kratos%E9%A3%9F%E7%94%A8%E8%AF%B4%E6%98%8E%E4%B9%A6.ini)
* [Wiki](https://github.com/ChrisLv-CN/DPKratos-Lite/wiki)

开发者 (Developers)
------------
* [艾木魁](https://space.bilibili.com/194846) (M.Kenosis) - 主策划
* [双杀步枪](https://space.bilibili.com/276838) (ChrisLv_CN) - 开发者

鸣谢 (Credits)
------------
* [DynamicPatcher](https://github.com/Xkein/YRDynamicPatcher) ALL developers
* Ares ALL developers
* [Phobos](https://github.com/Phobos-developers/Phobos) ALL developers
* [hejiajun107](https://github.com/hejiajun107) - 提供战机区域警戒功能
* [RA2DIY](https://bbs.ra2diy.com/) 红警2Mod开发私人会所

要饭 (Funding)
------------
如果你喜欢本项目，并想通过资助来帮助本项目，可以通过以下方式。  
If you like this project and want to fund it, here's how you can do it. 
* PayPal - 12737@live.com
* 支付宝 - [Alipay](https://github.com/ChrisLv-CN/YRDynamicPatcher-Kratos/blob/main/Images/alipay.jpg)
* 微信 - [Wechat](https://github.com/ChrisLv-CN/YRDynamicPatcher-Kratos/blob/main/Images/wechat.jpg)
* 爱发电 - [Afdian](https://afdian.net/@chrislv)

如何使用脚本（How to use a Script）
------------
1. 将编译好的脚本对应的`.pkg`文件放入`DynamicPatcher\Packages\Build\Scripts`。  
Put the `.pkg` file corresponding to the compiled script into `DynamicPatcher\Packages\Build\Scripts`.

2. 使用文本编辑器编辑`DynamicPatcher\Packages`下的`release.list`文件，在末行加入`{DP_DIR}\Build\Scripts\***.tmp`，`***`为脚本.pkg的文件名。  
Use a text editor to edit the `release.list` file in folder `DynamicPatcher\Packages`, and add `{DP_DIR}\Build\Scripts\***.tmp` in the last line. `***` is the file name of the script file of `.pkg`.

3. 启动游戏。  
Run.

如何编译脚本（How to compile Scripts)
------------
1. 正确安装并启动Kratos，确保Kratos运行正常。  
Install and start Kratos correctly to ensure that Kratos operates normally.

2. 从[源代码项目](https://github.com/ChrisLv-CN/DPKratos-Lite-Source)中获取Debug版本的`DynamicPatcher.dll`，替换。  
Get the Debug version of `DynamicPatcher.dll` from the [source code project](https://github.com/ChrisLv-CN/DPKratos-Lite-Source) and replace it.

3. 在文件夹`DynamicPatcher`下创建文件夹`Scripts`，并将写好的`.cs`脚本文件放进去。  
Create the folder 'Scripts' under the folder' DynamicPatcher 'and put the written `.cs` script file in it.

4. 启动游戏。  
Run.

5. 在`DynamicPatcher\Packages\Build\Scripts`中获得编译并打包好的`.pkg`文件。  
Get the compiled and packaged `.pkg` file in `DynamicPatcher\Packages\Build\Scripts`.
