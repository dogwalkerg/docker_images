# 教程
https://www.freedidi.com/14712.html
然后本地安装webUI

(1)在CPU下运行：

docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
 

(2)支持GPU运行：

docker run -d -p 3000:8080 --gpus=all -v ollama:/root/.ollama -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:ollama
 

安装完成通过本地地址：http://127.0.0.1:3000 进行访问，然后在里面下载安装Llama 3.2 模型
