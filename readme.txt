
docker run -d --rm -v /home/cci/Desktop/data/:/data zipcrack:1 sh -c "python crack.py -i /data/testPrint.zip 1 6 0123456789 >> /data/log.txt"