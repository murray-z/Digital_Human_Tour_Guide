# Digital_Human_Tour_Guide

数字人导游，以三苏祠为例

# 项目简介

- 本项目基于awesome-digital-human-live2d和dify搭建数字人导游项目，以三苏祠为例，实现数字人导游功能。
- 包含语音识别ASR、语音合成TTS、大模型对话LLM、知识库RAG、数字人等技术。

# 依赖项目

- [dify](https://github.com/langgenius/dify)
- [awesome-digital-human-live2d](https://github.com/wan-h/awesome-digital-human-live2d)
- [图片背景](https://www.sscbwg.com/)

# 实现步骤

1. 部署awesome-digital-human-live2d项目

```
step1:
git clone https://github.com/wan-h/awesome-digital-human-live2d.git

step2:
cd awesome-digital-human-live2d

step3:
下载三苏祠图片，添加图片到awesome-digital-human-live2d/web/public/backgrounds目录下并在awesome-digital-human-live2d/web/app/lib/live2d/lappdefine.ts中修改字段BackImages添加图片名称即可


step4:启动容器
# 项目根目录下执行
docker-compose up --build -d
```

2. 部署dify项目

```shell
setp1:
git clone https://github.com/langgenius/dify.git

step2:
cd dify
cd docker
cp .env.example .env
docker compose up -d
```

3. 在dify搭建对话流程
   ![dify流程图](./assets/dify.png)
4. 示例知识库文件

- [三苏祠知识库](./assets/三苏祠.docx)

# 效果展示

https://github.com/user-attachments/assets/ec1b17c3-a908-46b1-bf02-4326ebb29769

# 知识库校验

- ![占地面积](./assets/question1.png)
- ![门票](./assets/question2.png)
