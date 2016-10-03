# yun_deploy
服务器部署记录

## 安装git

url：https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

```
sudo yum install curl-devel expat-devel gettext-devel openssl-devel perl-devel zlib-devel
sudo yum install asciidoc xmlto docbook2X
wget https://www.kernel.org/pub/software/scm/git/git-2.10.0.tar.gz
tar -zxf git-2.10.0.tar.gz
cd git-2.10.0
make configure
$ ./configure --prefix=/usr
$ make all doc info
$ sudo make install install-doc install-html install-info


```

- 报错处理方法

```
cd /usr/local/src/
wget http://ftp.gnu.org/pub/gnu/libiconv/libiconv-1.14.tar.gz
tar -zxvf libiconv-1.14.tar.gz
cd libiconv-1.14
./configure -prefix=/usr/local/libiconv  &&  make  && sudo  make install
cd /usr/local/src/git-2.10.0
make configure
./configure --prefix=/usr/local -with-iconv=/usr/local/libiconv
make
make install
```
## 安装node

url:http://www.jianshu.com/p/c958bd3c7d77/comments/2946334
