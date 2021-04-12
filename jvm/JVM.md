<h1 align="center">虚拟机</h1>
<pre>
问题：java 出现could not open jvm.cfg 
原因：是由于卸载jdk 不干净而引起的.
方案：
一、在点击开始【运行】输入【regedit】确定打开注册表。
二、找到HKEY_LOCAL_MACHINE/software/javasoft，把这个javasoft删除即可。
javasoft正常情况下至少包含\Java Development Kit，Java Plug-in，Java Runtime Environment这三项，不用怕，删除Javasoft就会把这三项都删除，问题本身也是出在这里，所以需要删除javasoft项。

三、重装JDK（如果不改变文件位置都选默认，那是最好不过的啦！）重装后会发现，重新有一个HKEY_LOCAL_MACHINE/software/javasoft项，这是这些参数都是新的了，不会出现问题了。

</pre>