# -DeepSeek-RagFlow-Docker-
复现基于DeepSeek大模型的个人数据库搭建，基础来自于https://github.com/infiniflow/ragflow?tab=Apache-2.0-1-ov-file。本项目采用工具有RagFlow、Docker、Ollama）
本篇是自己复现个人数据库搭建后，对于一些流程及问题的记录。
一、Ollama下载
1.下载
登录Ollama官网
注意：从官网下载OllamaSetup.exe安装包后，不要直接双击运行。打开安装包所在的文件夹，在地址栏输入cmd并回车，快速唤起命令行窗口。
OllamaSetup.exe /DIR="D:\Ollama"
这里就会下载到D盘，后边完全就是正常安装。
2.测试
Windows命令行中执行curl http://127.0.0.1:11434，或者登录网址，出现下图即为连接成功
<img width="438" height="161" alt="ollama" src="https://github.com/user-attachments/assets/241b7812-f465-4744-a873-1ed85a63bcc7" />

二、Docker下载
1.下载
这里下载步骤
<img width="1076" height="283" alt="docker1" src="https://github.com/user-attachments/assets/75344869-a69f-415d-b969-0292721fe323" />
<img width="1516" height="1264" alt="docker2" src="https://github.com/user-attachments/assets/3cfac50d-58e9-4e1b-904f-7bac8e7c07c2" />
注：在这一步，我同样没有在c盘安装，这里步骤跟的是https://blog.csdn.net/Gwumingzhibei/article/details/160914283?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-0-160914283-blog-160013395.235^v43^pc_blog_bottom_relevance_base8&spm=1001.2101.3001.4242.1&utm_relevant_index=3
具体步骤如下：
start /w "" "Docker Desktop Installer.exe" install --installation-dir="D:\Docker\Program" --wsl-default-data-root="D:\Docker\Data"
2.WSL2
这个地方建议直接用cmd去查看，我是直接用的wsl --update，会直接更新最新的。

三、RagFlow登录
四、创建项目
