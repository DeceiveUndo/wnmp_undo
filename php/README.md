# PHP

## 下载

请到 [windows.php.net](http://windows.php.net/download/) 下载最新版的 `PHP for Windows`

`FastCGI` 安全
`Non Thread Safe` 非安全 


## 安装

解压下载包

进入根目录复制 `php.ini-development` 为 `php.ini`

编辑 `php.ini`，修改以下几个参数：

```ini
;extension_dir =“ext” 修改为 extension_dir=“ext” 把符号去掉
;extension=mysqli 修改为 extension=mysql 把符号去掉

```
启用扩展，定位到 `extension`，根据需要取消相关注释

然后打开终端定位到根目录
`.\php-cgi.exe -b 127.0.0.1:9000 -c php.ini`
如果没报错在闪就证明成功了

##Bat
绝对路径`\php-cgi.exe -b 127.0.0.1:9000 -c php.ini` 

