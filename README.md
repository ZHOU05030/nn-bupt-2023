# NNDL-bupt-2023

老登让设计图像描述任务的Encoder-Decoder框架神经网络

# 预期实现的两个框架

1. **CNN+GRU**：

- **CNN**: 卷积神经网络（CNN）用于提取图像的整体特征。CNN通过多层卷积层处理图像
- **GRU**: 门控循环单元（GRU）是一种用于文本生成的循环神经网络。在这个结构中，GRU用来生成图像描述，基于CNN或ViT提取的特征。


2. **网格/区域表示、Transformer编码器+Transformer解码器**：

- **网格/区域表示**: 同上，图像被分割成多个区域或网格。
- **Transformer编码器+解码器**: 使用Transformer架构的编码器来处理图像特征，解码器则用于生成文本描述。这种结构允许模型在生成描述时有效地利用图像的所有区域。

# 评价指标
+ METEOR
+ ROUGE-L

# 开发环境

Python env: torch2.0.1+cu118, python 3.10+

IDE: VSCode

Code: Jupyter notebook