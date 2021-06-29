# ffmpeg

## 合并视频

[链接](https://blog.csdn.net/doublefi123/article/details/47276739)

1. 先创建一个文本文件 `filelist.txt`
~~~
file 'input1.mkv'
file 'input2.mkv'
file 'input3.mkv'
~~~
2. 执行
~~~
ffmpeg -f concat -i filelist.txt -c copy output.mkv
~~~

## RTMP推流

[链接](https://zhuanlan.zhihu.com/p/73984438)

~~~
ffmpeg -i ${input_video} -vcodec copy -an -f flv rtmp://${server}/live/${streamName}
~~~
