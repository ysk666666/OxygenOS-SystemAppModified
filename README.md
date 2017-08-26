# OxygenOS-SystemAppModified
氧OS系统App的微改，使之拥有氢OS的功能  

## 详细说明
本项目是一加3T(OnePlus 3T)手机，氧OS(OxygenOS)系统App的修改版，以实现OxygenOS的系统App能像氢OS(HydrogenOS)那样具有更多的本地化功能，诸如通话录音。 
修改版本的App是和手机系统对应的，必须要同版本的才可以使用。 

## 使用方法  
设备已经root！  
把项目中的apk复制到手机的"/system/priv-app/"里面，并修改权限为644(-rw-r--r--)，然后把对应的的apk文件添加一个后缀".bak"就可以了(主要是不让系统认为其是一个apk，然后还能保留一份备份，以备出错了恢复)。然后重启手机再测试一下就可以了。  

## 对照列表  
OPInCallUI---系统拨通电话后的逻辑（扬声器挂断输入数字等的），用上本"OPInCallUI_y.apk"文件后就可以实现手动的通话录音了
更多的修改版等待后续完成。  
Dialer---系统的拨号程序。此修改版打开了“右上角三点-设置-通话自动录音”设置项的入口。配合修改版的OPInCallUI，就可以完美的实现通话录音了。

## 额外说明  
目前master分支对应的是氧OS 4.1.7，即4.1.7分支。  
分支的名字对应的就是氧OS的版本号，如果master分支没有，可以去相应的分支找找看。  
具体反编译的方法我也专门写了一篇博客，[博文链接](http://www.cnblogs.com/ysk-china/p/7162203.html)  
有什么意见或建议给我提issue就好了。