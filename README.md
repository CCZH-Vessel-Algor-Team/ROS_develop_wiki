# ROS 开发 Wiki

面向船舶与机器人开发的 ROS 2 技术资料库，整理开发调试、定位与姿态处理，以及 Navigation2 的对象模型、运行机制和工程接入方法。

技术文档见 [项目 Wiki](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki)。

## 文档入口

### 1. ROS2 开发与调试

| 文档 | 内容 |
| --- | --- |
| [ROS2 跨机通信配置](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/ROS-2-跨机通信配置) | DDS 发现与数据传输、ROS 环境变量、网络与防火墙、虚拟机桥接排障。 |
| [ROS2 Bag 回放与格式转换](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/ROS2-bag) | 虚拟时钟、循环回放，以及 SQLite Bag 转 MCAP 的示例。 |

### 2. 定位、姿态与传感器

| 文档 | 内容 |
| --- | --- |
| [robot_localization](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/robot_localization) | EKF/UKF、navsat_transform、datum，以及 map/odom/base_link 坐标体系。 |
| [姿态与旋转](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/姿态与旋转) | RPY 内禀/外禀旋转、旋转矩阵、Heading 与 Yaw；四元数章节待补充。 |
| [姿态传感器校准](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/姿态传感器校准) | Windows 上位机下的时间、加速度计、磁场、高度与陀螺仪校准操作记录。 |

### 3. Navigation2

[查看 Navigation2 分类目录](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Home#navigation2)

#### Costmap

| 文档 | 内容 |
| --- | --- |
| [Nav2 Costmap基础与工程接入](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Costmap-Integration) | 基础概念、LaserScan、Keepout Filter 与 Vector Object Server 接入。 |
| [Nav2 Costmap对象模型与运行机制](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Costmap-Architecture) | 核心对象持有关系、生命周期、更新线程和算法读写同步。 |

#### Controller

| 文档 | 内容 |
| --- | --- |
| [Nav2 Controller Server执行流程](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Controller-Server) | FollowPath 主循环与 computeAndPublishVelocity 子流程的时序速览。 |
| [Nav2 Controller体系与路径处理](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Controller-Path-Handling) | 插件接口、机器人状态输入、路径裁剪、坐标变换与碰撞检测。 |

#### Behavior 与导航任务

| 文档 | 内容 |
| --- | --- |
| [Nav2 Behavior机制与插件开发](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Behavior-Plugins) | BT 客户端与 Behavior 服务端解耦、状态传播和插件开发文件清单。 |
| [Nav2目标到达、运动进展与导航反馈](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Goal-Progress-Feedback) | Goal Checker、Progress Checker、两层 action feedback 与 RViz 显示。 |
| [Nav2多路点导航机制](https://github.com/CCZH-Vessel-Algor-Team/ROS_develop_wiki/wiki/Nav2-Multi-Pose-Navigation) | 目标数组推进、分段规划、路径拼接与动态目标替换。 |

## 历史更新

| 日期 | 维护者 | 文件 | 更新 |
| --- | --- | --- | --- |
| 2026-09-22 | vectorwang | Home.md | 整理分类目录。 |
| 2026-09-22 | vectorwang | _Sidebar.md | 新增侧边栏导航。 |
| 2026-09-22 | vectorwang | Nav2-Costmap-Integration.md | 新增 Costmap 基础与工程接入。 |
| 2026-09-22 | vectorwang | Nav2-Costmap-Architecture.md | 新增 Costmap 对象模型与运行机制。 |
| 2026-09-22 | vectorwang | Nav2-Controller-Server.md | 新增 Controller Server 执行流程。 |
| 2026-09-22 | vectorwang | Nav2-Controller-Path-Handling.md | 新增 Controller 体系与路径处理。 |
| 2026-09-22 | vectorwang | Nav2-Behavior-Plugins.md | 新增 Behavior 机制与插件开发。 |
| 2026-09-22 | vectorwang | Nav2-Goal-Progress-Feedback.md | 新增目标到达、运动进展与导航反馈。 |
| 2026-09-22 | vectorwang | Nav2-Multi-Pose-Navigation.md | 新增多路点导航机制。 |
| 2026-02-08 | vectorwang | ROS2-bag.md | ROS2 Bag 笔记。 |
| 2026-02-07 | vectorwang | 姿态与旋转.md | 姿态与旋转笔记。 |
| 2026-02-06 | vectorwang | robot_localization.md | ROS2 robot_localization 笔记。 |
| 2026-01-20 | vectorwang | ROS-2-跨机通信配置.md | ROS2 跨机通信配置。 |
