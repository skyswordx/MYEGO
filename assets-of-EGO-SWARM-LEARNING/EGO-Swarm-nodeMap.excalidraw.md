---

excalidraw-plugin: parsed
tags: [excalidraw]

---
==⚠  Switch to EXCALIDRAW VIEW in the MORE OPTIONS menu of this document. ⚠== You can decompress Drawing data with the command palette: 'Decompress current Excalidraw file'. For more info check in plugin settings under 'Saving'


# Excalidraw Data

## Text Elements
/random_forest ^T64ChIit

程序首先用这个节点生成了全局地图 ^JrY89kpD

并传递给各个无人机
负责激光雷达模块的节点  ^ca5KYPQR

/drone_${id}_pcl_render_node ^Ltkusrm1

这个节点负责模拟激光雷达，把接收到全局地图中
该无人机当前位置周围的障碍物点云信息发给规划器节点 ^tlCay2MX

/drone_${id}_ego_planner_node ^dW2eUVry

/drone_${id}_traj_server ^CGg2geAZ

这个节点完成和其他无人机的通信
并根据其他无人机的 B样条轨迹、障碍物信息和自身无人机状态
使用 EGO-Swarm 规划出均匀 B 样条轨迹 ^CnObAixc

这个节点负责把 B 样条轨迹转换成
具体的位姿控制指令 ^1kEOFkir

/drone_${id}_poscmd_2_odom ^x6Iy59e1

/drone_${id}_odom_visualization ^iYmrbGJc

这个节点负责模拟无人机接收控制指令并执行
发布无人机位姿以及里程计给各个节点 ^WNMzKQgC

这个节点接收里程计数据发负责无人机路线的可视化 ^qhOCkL6K

/map_generator/global_cloud ^ROC1ymJa

/${node_name}/cloud ^EqfuuT5i

/drnoe_${id}_planning/bspline ^72rYxqU0

/broadcast_bspline ^fxjiLGca

其他无人机的 ego_planner_node ^ZNUn1k0J

/broadcast_bspline ^kYZ5mghg

自己的 ego_planner_node 的反馈 ^RsW2Gn4l

/drnoe_${id}_planning/pos_cmd ^d1mUwjkp

/drnoe_${id}_visual_slam/odom ^QGeM7oiD

%%
## Drawing
```compressed-json
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
```
%%