# gm-Localization_generation
Gamemaker本地化生成,简单讲就是将给定目录gml文件读一遍,取出特定函数名的参数保存为csv

使用方法更简单了,将yyp拖到 `Gamemaker本地化生成.exe` 即可

或者直接将exe放入工程根目录运行

当进程关闭后会生成配置文件,下次你可以直接运行该exe

遍历时抓取的函数大概这样子: 
````
Lset("角色.年龄","24")
````
值得注意的是不可以换行,不可以用@""

转义也不会自动转换,跟直接在游戏内使用略有不同

需要加载时进行额外代码转义


配置文件大概这样
````
savePath="E:\project\Gamemaker本地化生成\dist\";
saveFileName="def.csv";
function_name="Lset";
projectPath="F:\Users\yunzl\Documents\GameMakerStudio2\test\"
````
或许你会希望文件直接生成在工程的datafiles内,你就可以修改savePath

目前就这些,等有时间了组装一个整体方案
