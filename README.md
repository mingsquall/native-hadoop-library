# native-hadoop-library
关于Hadoop2.7.3在Mac OS下运行时提示的警告：

*WARN util.NativeCodeLoader: Unable to load native-hadoop library for your platform... using builtin-java classes where applicable*

解决方法：使用此repository提供编译后的2.7.3的native-library，替换到目标hadoop-2.7.3/lib/native文件夹下即可。


+ 记得「hadoop checknative -a」命令来检查本地库加载情况。

##若成功，应显示：
>Native library checking:

>hadoop:  true /Users/patientman/Downloads/hadoop-2.7.3/lib/native/libhadoop.dylib

>zlib:    true /usr/lib/libz.1.dylib

>snappy:  true /usr/local/lib/libsnappy.1.dylib

>lz4:     true revision:99

