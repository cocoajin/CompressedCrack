# CompressedCrack

Compressed Crack is a simple tool to help you crack password zip and rar files.

## Use in Docker

```bash
# build docker image
build -t zipcrack:1 .

# run in background

docker run -d -v /Users/cc/Desktop/srcd:/data zipcrack:1 \
    python crack.py -i /data/test.zip 4 4 "0123456789"

```



## Requirements:

[Python 3.x](https://www.python.org/downloads/)

## Install

```
apt-get -y install git
git clone https://github.com/thanhminh6996/CompressedCrack.git
cd ./CompressedCrack
```
## Use
```
python crack.py -i INPUT [rules [rules ...]]

positional arguments:
  rules                 <min> <max> <character>

optional arguments:
  -h, --help            show this help message and exit
  -i INPUT, --input INPUT
                        Insert the file path of compressed file
                        
```                       
