KrkrExtract[Ver 0.0.0.5a]

Author:X'moe
目前提供krkr2和krkrz（包括M2公司）通用提取

使用方式：
一、提取封包：
将原始游戏exe（或者破解后能运行的exe）拖进KrkrExtract.exe进行加载
在这之前请关闭杀软之类的软件（特别是大数字）
如果成功后，会自动生成一个窗口，你现在可以把xp3文件拖进来进行拆包。
（最好是等游戏停留在title处开始拆包）
拆包后的文件在outPath里面。（现在的版本不用每解一个包就关一次游戏）

二、封装文件：
封包的时候，需要依次收集三个信息：
1.封包的目录（该目录下不应该有子目录，做过Krkr游戏汉化的人都知道是怎么回事）
2.输出文件名字（可以自己填写一个，比如temp.xp3。如果是用于汉化游戏，到时候可以依次改名为patch2.xp3...）
3.用于收集信息的游戏原始封包（最好选一个封包体积比较小的xp3，如果该封包有问题，
将会提示无法收集到足够的信息，这个时候你应该换一个封包试试，如果你确认这个是程序问题，可以给我发邮件）
上面三步完成以后，就可以开始打包。窗口顶部将会显示一个进度条。
如果没有任何错误发生，程序将会提示打包成功。

打包完成后，如果提示你关闭游戏，删除KrkrzTempWorker.xp3以打包下一个文件夹的话，
一定要按这个提示去做，要不然是封装不了的。

Support:
xmoe.project@gmail.com

[Note]
For long-term support, this project won't be an open source project at present.

[Dev log]
Version 0.0.0.5b  
Supported Multi_Language(CHS CHT JP EN)  

Version 0.0.0.5a  
ADD KrkrLoader Project's core   

Version 0.0.0.4g    
Fixed some bugs  

Version 0.0.0.4e  
Supported packing new format package  

Version 0.0.0.4d  
Fixed some errors  

Version 0.0.0.4c:  
Support one more GAME!  
neko~neko~moe~nya~  

Version 0.0.0.4b  
Fixed some bugs when extract psb files

Version 0.0.0.4a  
See ReadMe

Version 0.0.0.3d  
（非常重要的更新!!）
解决了x公司krkrz后期加密的改动，理论上完全通用了。
已经在魔女的夜宴和feng的新作上（说这句话的时候是2015.9.11）实验成功了。
打包完成后，如果提示你关闭游戏，删除KrkrzTempWorker.xp3以打包下一个文件夹的话，
一定要按这个提示去做，要不然是封装不了的。


Version 0.0.0.3c  
解决部分Krkrz封包识别错误的问题。


Version 0.0.0.3b  
解决上一版本，某些游戏会封包失败的问题。
ToDo：开始完善Exe中的追加提取功能。

Version 0.0.0.3a:  
支持提取带“早期傻逼保护”的xp3封包。
自动分析部分未知数据。
支持封包！支持普通的krkr2和krkrz的xp3格式封包（含加密），
支持特殊格式的krkrz封包（含加密，如柚子社的サノバウィッチ）
暂时从Exe中移除特殊资源提取功能。

Version 0.0.0.2d:  
支持某些Chunk比较扭曲的游戏的提取。
目测是早期M2公司使用krkrz开发的作品。
下一版本增加封包工程。

Version 0.0.0.2c:  
添加对feng社游戏的支持。

Version 0.0.0.2b:  
添加对“某些”游戏的支持。


Version 0.0.0.2a:  
修正提取bug，支持未知Chunk的分析。
改进提取线程。
内置IA32反编译器引擎，用于分析加密流程（目前暂时没开放这个功能）
内置LE Mudole，如果你系统默认的CodePage不是日区的，在提取某些krkrz开发的游戏时，
部分提取可能会失败。KrkrExtract会自动启动LE Module。

给KrkrExtract.exe增加功能：
在无额外参数启动的情况下（就是直接双击KrkrExtract.exe），会启动资源提取器。
Krkr相关的（如*.psb *.scn *.tlg *.pimg）资源可以进行提取。
目前支持TLG5/6的提取
*.PSB *.SCN 二进制脚本的反编译


Version 0.0.1.a:  
添加进度。
在提取多个文件的时候，不必重启游戏（但是不能同时提取多个文件，请依次拖放）

Todo：  
M2公司某些xp3压缩包中的某些文件可能会提取失败，正在找解决办法。


Test Release:

Todo：  
目前不支持Loader的加载（详见注释1）


注释：
①有的游戏包括原版游戏是用Loader机制加载的，特别是汉化版游戏。
为了保护汉化补丁，将不会支持这种游戏的提取。