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
