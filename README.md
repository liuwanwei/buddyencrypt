#### 在 Linux、macOS 上编译
```
git clone https://github.com/lihancong/tonyenc.git
cd tonyenc
phpize
./configure
make
```
将编译好的文件 modules/tonyenc.so 加入到配置项 extension=tonyenc.so，重启 PHP 服务

## 加密

代码中的 `~/php/tonyenc.php` 是加密工具:
```bash
php ~/php/tonyenc.php example.php dir/
```
这样即可加密 `example.php` 和 `dir` 目录下的所有 php 文件，PHP 在运行它们时会自动解密，够简单吧！
