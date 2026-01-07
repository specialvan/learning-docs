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
    * [openai/CLIP](https://github.
