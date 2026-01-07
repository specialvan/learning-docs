第一周：概念构建与仿真基础
目标：理解什么是具身智能，学会看机器人“模型文件”。

周一：全局视野

阅读：awesome-embodied-ai 的 README。

任务：搞清楚 VLM（视觉语言模型）和 VLA（视觉语言动作模型）的区别。

周二：物理引擎入门

阅读：MuJoCo Documentation 的 Getting Started。

任务：理解什么是 Rigid Body Dynamics（刚体动力学）。

周三：认识机器人身体 (URDF)

阅读：搜索 GitHub 上的 franka_description 或 kinova_description 仓库。

任务：在 urdf 文件夹里找 .urdf 文件，看明白 link（连杆）和 joint（关节）是如何定义的。

周四：仿真平台实操观摩

阅读：NVIDIA IsaacGymEnvs。

任务：看它的 docs/ 里的环境列表，了解如何模拟成千上万只蚂蚁走路。

周五：周总结与视频解压

任务：在 GitHub 仓库里搜 Issue 或 Discussions，看大牛们在讨论什么 Bug。

📅 第二周：大脑模型 (VLA & Foundation Models)
目标：理解现在最火的“大模型控场”是怎么回事。

周一：RT-1 & RT-2 理论

阅读：google-research/robotics_transformer。

任务：理解“Tokenization of Actions”——如何把动作像文字一样编码。

周二：OpenVLA 深度解析

阅读：openvla/openvla。

任务：看 model.py 结构（按 . 键进入 VS Code 模式），看它是怎么把图像特征和文字特征融合的。

周三：数据协议 RLDS

阅读：google-research/rlds。

任务：了解机器人的一条“轨迹”（Trajectory）包含哪些数据（Step, Observation, Action, Reward）。

周四：跨模态对齐

阅读：CLIP 的 README（这是具身智能视觉部分的基石）。

任务：理解图像和文字如何在向量空间里“碰头”。

周五：大模型微调逻辑

阅读：LeRobot 的 Train a Model 章节。

📅 第三周：动作策略 (Policy) 与算法
目标：研究机器人具体是怎么“动”起来的。

周一：模仿学习 (BC)

阅读：robomimic 的入门文档。

任务：理解 Behavior Cloning（行为克隆）的基本公式。

周二：扩散策略 (Diffusion Policy)

阅读：columbia-ai-robotics/diffusion_policy。

任务：看它的训练配置，理解为什么它比传统的强化学习更稳。

周三：强化学习实战 (PPO)

阅读：CleanRL 里的 ppo.py。

任务：这被称为“最干净的 PPO 实现”，注释非常多，适合带薪阅读。

周四：手眼协调 (Hand-eye Coordination)

阅读：Universal Manipulation Interface (UMI)。

任务：研究如何通过一个普通摄像头（GoPro）实现高精度操作。

周五：算法对比

任务：在 awesome-embodied-ai 找一张算法对比表，存入你的笔记。

📅 第四周：硬件、ROS 与工程落地
目标：从纯算法转向真实的机器工程。

周一：ROS 2 基础概念

阅读：ros2/ros2。

任务：理解什么是 Node（节点）、Topic（话题）和 Service（服务）。

周二：硬件选型摸鱼

阅读：Mobile ALOHA 的硬件清单（BOM）。

任务：去搜搜什么是 Dynamixel 电机，它们是怎么通讯的。

周三：实时操作系统 (RTOS) 概念

阅读：GitHub 上关于 Preempt-RT 的讨论。

任务：理解为什么机器人控制需要“毫秒级”的确定性。

周四：工业级应用 Case

阅读：Anybotics/elevation_mapping。

任务：看四足机器人是如何在不平整地面导航的。

周五：撰写你的“技术报告”

任务：汇总这四周的 MD 笔记，假装正在为公司写一份《具身智能技术调研报告》。
