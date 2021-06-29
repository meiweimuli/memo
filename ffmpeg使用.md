# ffmpeg使用

## 合并视频

https://blog.csdn.net/doublefi123/article/details/47276739

先创建一个文本文件 filelist.txt
~~~
file 'input1.mkv'
file 'input2.mkv'
file 'input3.mkv'
~~~
然后
~~~
ffmpeg -f concat -i filelist.txt -c copy output.mkv
~~~
