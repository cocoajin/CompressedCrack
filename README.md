# CompressedCrack

Compressed Crack is a simple tool to help you crack password zip and rar files.

## Use in Docker

```bash
# build docker image
docker build -t zipcrack:1 .

# run in background

docker run -d -v /Users/cc/Desktop/srcd:/data zipcrack:1 python crack.py -i /data/test.zip 4 4 "0123456789"

docker run -d --rm -v /home/cci/Desktop/data/:/data zipcrack:1 sh -c "python crack.py -i /data/testPrint.zip 1 6 0123456789 >> /data/log.txt"

```


## Use rules

```
python crack.py -i INPUT [rules [rules ...]]

positional arguments:
  rules                 <min> <max> <character>

optional arguments:
  -h, --help            show this help message and exit
  -i INPUT, --input INPUT
                        Insert the file path of compressed file
                        
```                       
