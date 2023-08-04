If a directory named portable_config next to the mpv.exe exists, all config will be loaded from this directory only. 

Config files located in the same directory as mpv.exe are loaded with lower priority. Some config files are loaded only once, which means that e.g. of 2 input.conf files located in two config directories, only the one from the directory with higher priority will be loaded.

A third config directory with the lowest priority is the directory named mpv in the same directory as mpv.exe. This used to be the directory with the highest priority, but is now discouraged to use and might be removed in the future.

配置文件可以存放在多个地方, 按照读取配置文件的优先级排列如下:
1. 与 mpv.exe 同级的目录, 可以创建一个 portable_config 文件夹, 里面防止放置配置文件和脚本文件
2. %AppData%/mpv/
3. 与 mpv.exe 同级目录下
4. 与 mpv.exe 同级目录下的 mpv 文件夹内(不推荐使用此设置, 并且此功能在后续版本中可能会移除)

配置文件只会读取一次, 只读取优先级高的一个.
