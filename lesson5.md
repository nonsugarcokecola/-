# 笔记（作业在下方）

### 阅读笔记：大模型部署的理论与实践

#### 一、大模型部署背景与挑战

- **背景介绍**：概述大模型部署的背景和实践环节。
- **计算与显存问题**：讨论实际部署中所需的计算能力和显存问题。
- **仿存瓶颈**：分析大模型推理过程中的仿存瓶颈问题及其解决方案。

#### 二、减少模型参数的方法

- **非结构化与结构化**：介绍减少模型参数的非结构化和结构化方法。
- **知识蒸馏**：讲解通过知识蒸馏降低训练难度的方法。
- **模型量化**：讨论模型量化提高计算效率和减少内存占用的优势。
- **MD PL软件**：介绍MD PL软件的三个核心功能。

#### 三、MD集成与环境配置

- **集成MD**：如何在Python中集成MD，并比较MDEP与transformer库的推理速度。
- **INTEL平台配置**：介绍在INTEL平台上创建和配置MD环境的方法。
- **HugFace社区**：提及HugFace作为深度学习模型和数据集的在线托管社区。

#### 四、模型对话与量化

- **终端对话**：展示如何使用Python终端与模型进行对话。
- **量化过程**：演示模型量化的过程，包括设置kv catch缓存大小和使用自动AWQ算法。

#### 五、模型量化与API服务

- **量化模型API**：介绍如何将量化后的模型作为API服务提供给客户端。
- **客户端访问**：介绍客户端调用API服务的方式。
- **量化服务功能**：介绍V的量化服务功能，包括本地部署和大模型封装为API服务器。

#### 六、端口转发与模型集成

- **端口转发**：讲解如何通过命令行进行端口转发。
- **Python代码集成**：介绍如何使用Python代码集成MD模型。

#### 实际部署中的挑战

- **计算量**：大模型部署时面临的计算量问题。
- **内存开销**：内存资源的开销问题。
- **仿存瓶颈**：存储访问速度限制导致的瓶颈。
- **用户请求不确定性**：用户请求的不可预测性对部署的影响。



# 作业

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

