# 🤖 具身智能 (Embodied AI) 四周学习进阶计划

> **阅读建议**：在 GitHub 页面按下键盘上的 `.` 键，使用 Web 版 VS Code 阅读，排版更专业。

---

## 🟢 第一周：概念构建与仿真基础
**目标**：理解具身智能的定义，学会看机器人的“身体描述”文件。

* **周一：全局视野与术语对齐**
    * [awesome-embodied-ai](https://github.com/robotics-editing/awesome-embodied-ai)
    * **任务**：阅读 README，区分 VLM（离身）与 VLA（具身）的区别。
* **周二：物理引擎 —— 机器人的物理定律**
    * [google-deepmind/mujoco](https://github.com/google-deepmind/mujoco)
    * **任务**：了解 MJCF (XML) 格式如何描述重力、摩擦力和碰撞。
* **周三：URDF —— 机器人的“说明书”**
    * [ros/urdf](https://github.com/ros/urdf)
    * **案例**：[Panda 机械臂 URDF](https://github.com/frankaemika/franka_ros/blob/develop/franka_description/robots/panda_arm.urdf.xacro)
    * **任务**：理解 Link（连杆）和 Joint（关节）的父子级联关系。
* **周四：并行仿真 —— GPU 加速训练**
    * [NVIDIA-Omniverse/IsaacGymEnvs](https://github.com/NVIDIA-Omniverse/IsaacGymEnvs)
    * **任务**：了解如何利用 GPU 开启成千上万个并行训练环境。
* **周五：数据流闭环**
    * [huggingface/lerobot](https://github.com/huggingface/lerobot)
    * **任务**：理解一个 Step 包含：Observation(感知) -> Action(动作) -> Reward(奖励)。

---

## 🟦 第二周：大脑模型 (Foundation Models)
**目标**：理解大模型如何成为机器人的“指挥官”。

* **周一：RT-1/RT-2 理论**
    * [google-research/robotics_transformer](https://github.com/google-research/robotics-transformer)
    * **重点**：理解 Action Tokenization（动作词元化）。
* **周二：OpenVLA 通用模型**
    * [openvla/openvla](https://github.com/openvla/openvla)
    * **重点**：看模型如何处理“视觉+指令”并输出“动作控制”。
* **周三：数据协议 RLDS**
    * [google-research/rlds](https://github.com/google-research/rlds)
    * **重点**：学习标准化机器人轨迹数据的存储格式。
* **周四：视觉特征对齐 CLIP**
    * [openai/CLIP](https://github.com/openai/CLIP)
    * **重点**：理解图像和文本如何在同一个特征空间匹配。
* **周五：微调逻辑与实战**
    * [huggingface/lerobot](https://github.com/huggingface/lerobot)
    * **重点**：看 `examples/` 文件夹下如何加载预训练权重。

---

## 🟧 第三周：动作策略 (Action Strategy)
**目标**：研究机器人具体是怎么动得“像人一样”丝滑。

* **周一：模仿学习 (BC)**
    * [ARISE-Initiative/robomimic](https://github.com/ARISE-Initiative/robomimic)
    * **重点**：看 Behavior Cloning 算法如何从人类演示中学习。
* **周二：扩散策略 (Diffusion Policy)**
    * [columbia-ai-robotics/diffusion_policy](https://github.com/columbia-ai-robotics/diffusion_policy)
    * **重点**：理解去噪生成过程如何让动作更平滑、更稳定。
* **周三：强化学习 PPO**
    * [vwxyzjn/cleanrl](https://github.com/vwxyzjn/cleanrl)
    * **重点**：查阅 `ppo.py` 源码，了解“奖励函数”如何引导机器人。
* **周四：UMI 手眼协调**
    * [real-stanford/universal-manipulation-interface](https://github.com/real-stanford/universal-manipulation-interface)
    * **重点**：看项目如何通过 GoPro 摄像头捕获高精度操作数据。
* **周五：策略算法综合对比**
    * 回到 [awesome-embodied-ai](https://github.com/robotics-editing/awesome-embodied-ai) 查看 Policy 部分。

---

## 🟫 第四周：工程落地 (Engineering)
**目标**：从算法回归到真实的硬件、通讯与系统。

* **周一：ROS 2 核心通讯**
    * [ros2/ros2](https://github.com/ros2/ros2)
    * **重点**：理解节点 (Node)、话题 (Topic) 和服务端 (Service) 的交互。
* **周二：Mobile ALOHA 硬件解析**
    * [tonyzhaozh/aloha](https://github.com/tonyzhaozh/aloha)
    * **重点**：查看 `Hardware` 目录下的 3D 打印件和物料清单 (BOM)。
* **周三：实时系统与控制频率**
    * 搜索 GitHub 上的 `Preempt-RT` 或 `Control Loop` 讨论。
    * **重点**：为什么控制循环需要达到 100Hz 甚至 1000Hz。
* **周四：四足与导航案例**
    * [ANYbotics/elevation_mapping](https://github.com/ANYbotics/elevation_mapping)
    * **重点**：研究真实物理世界中的地形测绘与避障。
* **周五：学习总结报告**
    * 整理四周的阅读笔记，形成你自己的具身智能知识图谱。

---
