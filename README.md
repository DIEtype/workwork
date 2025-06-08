# workwork

本项目为学习练手和课程作业，旨在探索基于咳嗽音频和深度学习方法进行肺部疾病识别的可行性。使用的数据来源于公开的 Coswara 项目，模型采用 MLP 和 CNN-Transformer 融合架构构建，并以 COVID-19 检测为示例场景进行训练与评估。

⚠️ **声明**  
本项目仅用于课程学习与模型练习之目的，代码未经严格测试，仅供参考与交流，**不适用于临床或实际医学用途**。

## 内容简介

- 数据预处理与特征提取（结构化声学特征 + Mel频谱图）
- 多层感知机（MLP）建模
- CNN-Transformer 频谱图像建模
- 融合模型训练与评估（包括与 ResNet50 基线对比）
- 模型性能可视化：Loss 曲线、混淆矩阵、AUC 等

## 数据来源

本项目所用音频数据来自 [Coswara 项目](https://github.com/iiscleap/Coswara-Data)，由印度IISc团队公开发布，使用编号为20220116、20220224音频数据，遵循 CC BY-SA 4.0 许可协议。
本研究中，ResNet50 被用作基线图像分类模型。模型架构参考自 TensorFlow 官方维护的 [Models Repository](https://github.com/tensorflow/models/tree/master/research/slim)，并加载其 ImageNet 预训练参数。

## 环境要求

- Python 3.10+ / R
- TensorFlow / Keras
- scikit-learn
- librosa
- matplotlib, numpy 等
- table1，flextable，Hmisc等
