# 金庸小说人物词向量可视化

本项目使用Word2Vec模型对金庸小说中的人物进行词向量训练，并通过多种方式实现可视化展示。

## 项目结构

├── novels/                  # 金庸小说文本文件

├── characters_names_full.txt     # 人物名称列表

├── main.py                  # 主程序

├── word2vec.ipynb   # Jupyter Notebook版本

└── README.md                # 项目说明文档

其他文件未直接使用，仅存档备用

## 功能特点

1. **词向量训练**
   - 使用Word2Vec模型训练人物词向量
   - 支持自定义词向量维度、窗口大小等参数

2. **多种可视化方式**
   - Matplotlib静态可视化（2D和3D）
   - P5.js交互式3D可视化
   - Plotly交互式3D可视化

3. **数据处理**
   - 自动分词处理
   - 支持中文显示
   - PCA降维处理

## 环境要求

- Python 3.6+
- 主要依赖包：
  - jieba
  - gensim
  - numpy
  - matplotlib
  - sklearn
  - plotly

## 安装依赖

```bash
pip install jieba gensim numpy matplotlib scikit-learn plotly
```

## 使用方法

1. **准备数据**
   - 将金庸小说文本文件放入`novels`目录
   - 确保`characters_names.txt`包含需要分析的人物名称

2. **运行程序**
   ```bash
   python main.py
   ```

3. **查看结果**
   - Matplotlib可视化结果将保存为`characters_2d.png`和`characters_3d.png`
   - P5.js交互式可视化将生成`visualization.html`
   - Plotly交互式可视化将生成`characters_plotly.html`

## 可视化效果

1. **Matplotlib可视化**
   - 2D散点图展示人物关系
   - 3D散点图展示人物关系
   - 支持中文标签显示

2. **P5.js交互式可视化**
   - 支持鼠标拖动旋转视角
   - 支持滚轮缩放
   - 支持悬停显示人物名称

3. **Plotly交互式可视化**
   - 支持多种交互操作
   - 支持图例显示/隐藏
   - 支持保存图片

## 注意事项

1. 确保`novels`目录中的文本文件编码为UTF-8
2. 确保`characters_names.txt`中的人物名称正确
3. 对于P5.js可视化，建议使用本地服务器运行HTML文件
4. 对于中文显示，需要确保系统安装了中文字体

## 扩展建议

1. 可以尝试不同的词向量维度
2. 可以调整Word2Vec模型的参数
3. 可以添加更多的可视化方式
4. 可以增加人物关系的分析功能
