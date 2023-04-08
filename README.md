#  大佬的项目：https://github.com/CJReinforce/PikPakAutoOfflineDownloadBot 用法也在这里看！！！！！
docker部署：

1.web拉取wxg1015/pikpakbot:latest 或者ssh运行docker pull wxg1015/pikpakbot:latest

2.下载库里的所有文件并解压放进code文件夹下然后编辑config.py进行配置并保存

3.将code目录复制到宿主机某路径下

4.nas系统web部署或ssh执行以下：

$ docker run \
  --name=pikpakbot \
  --restart=always \
  -d -v /路径/code:/code \
  wxg1015/pikpakbot:latest $
  
 
 写在最后：感谢CJReinforce大佬写的这个超好用的电报pikpak全自动机器人工具，我这里只是根据教程构建了镜像并上传至dockerhub外加写了个简易部署教程以方便大家，大神请无视·····
