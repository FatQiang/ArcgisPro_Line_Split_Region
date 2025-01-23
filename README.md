# 1 工具介绍

  该工具是基于ARCGIS PRO的model builder构建，可用于生成交通分析小区等。
  
  该工具主要流程为：【生成道路缓冲区】->【融合道路缓冲区】->【生成道路缓冲区中心线】->【分割区域】
  其中主要参数为【缓冲区距离】以及【清除悬挂线的阈值】，可根据实际情况调整该参数。
  【缓冲区距离】用于融合距离较近的道路，避免最后生成过小的区域。
  【清除悬挂线的阈值】用于生成道路缓冲区中心线之后，如果存在长度小于该阈值的悬挂线段，则删除该线段。
  
# 2 运行环境
  Arcgis pro
# 3 目录结构描述
    ├── Tool/GenerateTAZs.atbx //工具源文件
    ├── ReadMe.md           // 帮助文档
# 4 使用说明
## 4.1 加载工具
在Arcgis Pro中加载工具

![image](Images/Add_Tool_0.png)

在目录中选择模型文件

![image](Images/Add_Tool_1.png)

添加后工具箱中会显示GenerateTAZs工具

![image](Images/Add_Tool_2.png)

## 4.2 使用工具
数据准备，线数据以及待分割的面数据

![image](Images/Data_0.png)

打开工具，输入相应参数

![image](Images/Tool_Interface_0.png)

运行工具，查看生成结果

![image](Images/Result_0.png)
