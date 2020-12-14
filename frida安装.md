###vscode安装代码提示
npm i  @types/friad-gum

###安装启动

/data/local/tmp/frida-server

adb forward tcp:27042 tcp:27042

frida-ps -R

frida -U com.ss.android.ugc.aweme -l si.js


###如果无法启动关闭debuggable
adb shell //adb进入命令行模式
su //切换至超级用户
magisk resetprop ro.debuggable 1  //设置debuggable
stop;start; //一定要通过该方式重启
