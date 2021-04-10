<h1  align="center">IntelliJ IDEA 2018.3 x64 使用手册</h1>

<h3>一、控制台中文日志输出乱码</h3>
<pre>
（1）idea64.exe.vmoptions 、 idea64.exe.vmoptions在这两个文件内容的末尾分别添加：-Dfile.encoding=UTF-8
（2）【Run/Debug Configurations】 VM options： -Dfile.encoding=UTF-8
（3）【File】->【Settings】->【File Encodings】  
	Global Encodings：UTF-8
	Project Encodings：UTF-8
	Path->Encoding：UTF-8
	Default encoding for properties files：UTF-8
	Create UTF-8 files：with NO BOM
</pre>

<h3>二、war exploded</h3>
<pre>
问题：
Artifact exp3:war exploded: Error during artifact deployment. See server log for details.
解决：
【File】->【Project Structure】->【Artifacts】
出现黄色的波浪线异常提示，删除后重新添加【Web Application:Exploded】->【From Modules...】点击【Apply】
</pre>

<h3>三、添加lib如servlet-api.jar</h3>
<pre>
【File】->【Project Structure】->【Libraries】->【+】->【java】
选中D:\Program Files (x86)\java\apache-tomcat-8.5.65\lib\servlet-api.jar
</pre>