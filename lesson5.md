- 配置lmdeploy运行环境

![image-20240409191903108](lesson5.assets/image-20240409191903108.png)

- 下载internlm-chat-1.8b模型

![image-20240409191954426](lesson5.assets/image-20240409191954426.png)

- 以命令行方式与模型对话

![image-20240409192736565](lesson5.assets/image-20240409192736565.png)

## 进阶作业



完成以下任务，并将实现过程记录截图：

- 设置KV Cache最大占用比例为0.4，开启W4A16量化，以命令行方式与模型对话。（优秀学员必做）

0.8时

![image-20240409193525570](lesson5.assets/image-20240409193525570.png)

0.4时

![image-20240409193824741](lesson5.assets/image-20240409193824741.png)



- 以API Server方式启动 lmdeploy，开启 W4A16量化，调整KV Cache的占用比例为0.4，分别使用命令行客户端与Gradio网页客户端与模型对话。（优秀学员）

量化

![image-20240409194521973](lesson5.assets/image-20240409194521973.png)

启动客户端

![image-20240409195924014](lesson5.assets/image-20240409195924014.png)

命令行客户端

![image-20240409200247576](lesson5.assets/image-20240409200247576.png)

网页端客户端

![image-20240409200740674](lesson5.assets/image-20240409200740674.png)

- 使用W4A16量化，调整KV Cache的占用比例为0.4，使用Python代码集成的方式运行internlm2-chat-1.8b模型。（优秀学员必做）

![image-20240409201541856](lesson5.assets/image-20240409201541856.png)

- 使用 LMDeploy 运行视觉多模态大模型 llava gradio demo （优秀学员必做）

命令行

![image-20240409203508240](lesson5.assets/image-20240409203508240.png)



网页端/将 LMDeploy Web Demo 部署到 [OpenXLab](https://github.com/InternLM/Tutorial/blob/camp2/tools/openxlab-deploy) 

![image-20240409204616746](lesson5.assets/image-20240409204616746.png)


