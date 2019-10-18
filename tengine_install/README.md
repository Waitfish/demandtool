[toc]
## Download url
```bash
http://tengine.taobao.org/download/tengine-2.3.2.tar.gz
https://www.openssl.org/source/openssl-1.1.1d.tar.gz
https://ftp.pcre.org/pub/pcre/pcre-8.43.tar.gz
https://www.zlib.net/zlib-1.2.11.tar.gz
```

## Install 
```bash
rewrite << pcre
gzip << zlib
SSL modules << openssl
```

```bash
./configure --with-pcre=../pcre-8.43 --with-openssl=../openssl-1.1.1d  --with-zlib=../zlib-1.2.11
make
make install
```
## FAQ
### make error
```bash
configure: error: Invalid C++ compiler or C++ compiler flags
```
`yum install -y gcc gcc-c++`
