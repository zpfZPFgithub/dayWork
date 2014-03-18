
### Arcanist 安装
Arcanist 是phabricator的提交代码评审工具，不使用Arcanist也能使用Diffenential进行代码评审
方法是在web界面的Differential点击右上角“create diff”创建Diff和Revision。

但是“create diff“方式出现一个问题，作者create diff-》评审人提前审核通过，作者提交代码，diff依然留在web界面，没有关闭。
不知道是windows环境问题还是phabricator的一个bug。用Arcanist的方式该问题则不会出现。

windows下安装Arcanist的步骤
原文地址：
https://secure.phabricator.com/book/phabricator/article/arcanist_windows/
https://secure.phabricator.com/book/phabricator/article/arcanist/

需要的组件
1 PHP CLI 　这是因为Arcanist 使用php写的，Arcanist 运行在 PHP 5.2 或者更新版本中。下载链接：http://www.php.net/.
2 选择一个路径克隆以下文件
	1  git://github.com/facebook/libphutil.git
	2  git://github.com/facebook/arcanist.git
3 arcanist/bin添加到path环境变量中。 环境变量可以让操作系统找到你要执行的程序的地址
 我电脑的环境变量参考：c:\program files\imagemagick-6.5.2-q16;c:\program files (x86)\imagemagick-6.5.2-q16;C:\Program Files (x86)\NVIDIA Corporation\PhysX\Common;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Program Files (x86)\Microsoft SQL Server\90\Tools\binn\;C:\Program Files\Microsoft\Web Platform Installer\;C:\Program Files (x86)\Microsoft ASP.NET\ASP.NET Web Pages\v1.0\;C:\Program Files (x86)\Windows Kits\8.0\Windows Performance Toolkit\;C:\Program Files\Microsoft SQL Server\110\Tools\Binn\;D:\program_installed\bin;C:\Program Files\Microsoft SQL Server\110\DTS\Binn\;C:\Program Files (x86)\Microsoft SQL Server\110\Tools\Binn\;C:\Program Files (x86)\Microsoft SQL Server\110\Tools\Binn\ManagementStudio\;d:\program_installed\vs2010\Common7\IDE\PrivateAssemblies\;C:\Program Files (x86)\Microsoft SQL Server\110\DTS\Binn\;C:\Program Files\nodejs\;D:\php-5.3.10-ts-Win32-VC9-x64;D:\php-5.3.10-ts-Win32-VC9-x64\ext;C:\Users\Administrator\arcanist\bin;
 cmd下运行 arc 出现 Usage Exception: No command provided. Try 'arc help'。说明你成功了。
4 配置编辑器 $ arc set-config editor "\"C:\Program Files (x86)\Notepad++\notepad++.exe\" -multiInst -nosession"

<end>
arcanist 常用命令
cd d(进入c盘)
git checkout
arc diff



