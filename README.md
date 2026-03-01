# YOLOv8 人车目标检测系统

基于 YOLOv8 和 Faster R-CNN 的人车目标检测系统，集成 Streamlit Web 界面，支持图片上传检测、视频检测和实时摄像头检测，并提供多模型性能对比分析。

## 项目目的

利用深度学习目标检测算法（YOLOv8、Faster R-CNN）实现对道路场景中行人和车辆的自动识别与定位，为智能交通、自动驾驶辅助和城市监控等场景提供技术方案，并通过多模型对比验证检测效果。

## 核心功能

- **Streamlit Web 界面**：基于浏览器的可视化检测平台，操作简便
- **YOLOv8 目标检测**：使用 YOLOv8 实现高速人车检测
- **Faster R-CNN 对比**：提供 Faster R-CNN 模型的训练与评估结果
- **多模式检测**：支持图片上传、视频文件和摄像头实时检测
- **置信度调节**：可调整检测阈值控制检测灵敏度
- **性能评估**：提供 AP、Recall、Precision、F1 等完整评估指标

## 使用说明

### 环境安装

`ash
pip install streamlit ultralytics
`

### 启动 Web 检测界面

`ash
cd 1005/yolov8_qianduan
streamlit run app.py
`

## 项目结构

`
.
 1005/
     yolov8_qianduan/          # YOLOv8 检测前端
        app.py                # Streamlit 主程序
        config.py             # 模型配置
        utils.py              # 工具函数
        weights/              # 模型权重
        renche/               # 人车数据集（train/test/val）
        train/                # 训练脚本与配置
        requirements.txt      # 依赖列表
     frcnn/                    # Faster R-CNN 对比实验
         results/              # 评估结果（AP/Recall/Precision/F1）
         logs/                 # 训练日志
`

## 适用场景

- 智能交通监控与分析
- 自动驾驶辅助感知
- 城市安防视频分析
- 目标检测模型对比研究
- 深度学习 Web 应用开发学习

## 技术栈

| 组件 | 技术 |
|------|------|
| 目标检测 | YOLOv8, Faster R-CNN |
| Web 界面 | Streamlit |
| 深度学习 | PyTorch, ultralytics |
| 图像处理 | OpenCV, Pillow |

## License

MIT License
