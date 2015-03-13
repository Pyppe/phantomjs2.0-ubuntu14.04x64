# PhantomJS 2.0 built on Ubuntu 14.04 x64

This repository contains a PhantomJS 2.0 -binary for Ubuntu. It was compiled on a DigitalOcean 8GB Ubuntu 14.04 x64 -virtual machine. See [PhantomJS #12948](https://github.com/ariya/phantomjs/issues/12948) for details.

### Download
```bash
wget https://github.com/Pyppe/phantomjs2.0-ubuntu14.04x64/raw/master/bin/phantomjs
```

## What was done
```bash
apt-get update
apt-get install unzip
apt-get install build-essential g++ flex bison gperf ruby perl libsqlite3-dev libfontconfig1-dev libicu-dev libfreetype6 libssl-dev libpng-dev libjpeg-dev

mkdir phantomjs
cd phantomjs
wget https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.0.0-source.zip
unzip phantomjs-2.0.0-source.zip

cd phantomjs-2.0.0/
time ./build.sh
```

#### Time to build
```
real    31m12.068s
user    103m8.413s
sys     10m39.078s
```

#### md5 / sha1
```
5cc2f2bedb614be5b3b50945754d56a9  bin/phantomjs
a06b0f5e1f41520ca3c752afc75014f8be6bf4d8  bin/phantomjs
```
