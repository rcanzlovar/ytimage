# ytimage

## Download a high-quality version of a youtube video thumbnail.

YouTube thumbnails are often beautiful images in their own right, and you might
want to download one for a wallpaper. If you munge throug the HTML from a 
youtube page, you can find the file, usually called maxresdefault.jpg and 
then download it by a normal web browser. This script automates this, allowing
you to just pass in the URL of the youtube video. 

Attempt to get maxresdefault.jpg but if that doesn't work, get the next best copy hqdefault.jpg

```
$ ytimage.sh https://www.youtube.com/watch?v=wEiRKpflgQA
wget https://i.ytimg.com/vi/wEiRKpflgQA/maxresdefault.jpg --output-document=/home/rcanzlovar/Pictures/YTimages/YT_wEiRKpflgQA.jpg
--2019-07-11 09:24:28--  https://i.ytimg.com/vi/wEiRKpflgQA/maxresdefault.jpg
...
Proxy request sent, awaiting response... 200 OK
Length: 162580 (159K) [image/jpeg]
Saving to: “/home/rcanzlovar/Pictures/YTimages/YT_wEiRKpflgQA.jpg”

100%[===========================================================================>] 162,580      891K/s   in 0.2s    

2019-07-11 09:24:29 (891 KB/s) - “/home/rcanzlovar/Pictures/YTimages/YT_wEiRKpflgQA.jpg” saved [162580/162580]
```
