# 📅 具身智能学习进阶：第 2 - 4 周计划

## 🟦 第二周：大脑模型 (Foundation Models)
**目标**：理解大模型如何成为机器人的“指挥官”。

* **周一：RT-1/RT-2 概念**
    * [google-research/robotics_transformer](https://github.com/google-research/robotics-transformer)
    * **重点**：看 README 中的 Model Architecture 描述。
* **周二：OpenVLA 实战协议**
    * [openvla/openvla](https://github.com/openvla/openvla)
    * **重点**：阅读 `Project Website` 链接里的视频演示。
* **周三：数据格式 RLDS**
    * [google-research/rlds](https://github.com/google-research/rlds)
    * **重点**：了解如何记录机器人的每一步（Step）。
* **周四：视觉对齐 CLIP**
    * [openai/CLIP](https://github.com/openai/CLIP)
    * **重点**：理解文字标签是如何对应到图像特征的。
* **周五：Hugging Face 机器人库**
    * [huggingface/lerobot](https://github.com/huggingface/lerobot)
    * **重点**：看 `examples/` 文件夹里的训练脚本。

---

## 🟧 第三周：动作策略 (Action Strategy)
**目标**：研究机器人具体是怎么动得“像人一样”丝滑。

* **周一：模仿学习基础**
    * [ARISE-Initiative/robomimic](https://github.com/ARISE-Initiative/robomimic)
    * **重点**：阅读 `Introduction` 了解行为克隆。
* **周二：扩散策略 (Diffusion Policy)**
    * [columbia-ai-robotics/diffusion_policy](https://github.com/columbia-ai-robotics/diffusion_policy)
    * **重点**：看项目主页的 GIF，对比它与传统算法的区别。
* **周三：强化学习 PPO**
    * [vwxyzjn/cleanrl](https://github.com/vwxyzjn/cleanrl)
    * **重点**：看 `ppo.py` 的代码注释，这是业内最易懂的实现。
* **周四：UMI 手眼协调**
    * [real-stanford/universal-manipulation-interface](https://github.com/real-stanford/universal-manipulation-interface)
    * **重点**：看 Hardware 章节，了解摄像头如何捕捉动作。
* **周五：算法综合对比**
    * 回到 [awesome-embodied-ai](https://github.com/robotics-editing/awesome-embodied-ai) 查找对比图表。

---

## 🟫 第四周：工程落地 (Engineering)
**目标**：了解真实的硬件、系统和通讯。

* **周一：ROS 2 基础架构**
    * [ros2/ros2](https://github.com/ros2/ros2)
    * **重点**：搞清楚什么是 Node (节点) 和 Topic (话题)。
* **周二：ALOHA 硬件结构**
    * [tonyzhaozh/aloha](https://github.com/tonyzhaozh/aloha)
    * **重点**：看 `Hardware` 目录下的 3D 打印件和电机清单。
* **周三：实时系统优化**
    * 搜索：GitHub 上的 `Preempt-RT` 相关讨论。
    * **重点**：了解为什么机器人需要高频控制循环。
* **周四：自主导航案例**
    * [ANYbotics/elevation_mapping](https://github.com/ANYbotics/elevation_mapping)
    * **重点**：看四足机器人是如何感知地形凹凸的。
* **周五：总结与展望**
    * 写一份学习总结，存入你自己的 GitHub Repo。

---
