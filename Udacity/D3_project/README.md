# D3项目说明
## 项目目的
分析击球时使用左手、右手、双手对平均分数的影响

## 分析数据集
选择棒球数据，在做可视化之前，对数据集做了处理，清除avg和hr为0的数据。

## 设计方法
创建了svg画布，分别用身高和体重作为x轴，avg作为y轴，画出点图，图例B代表双手，L代表左手，R代表右手，分别用不同颜色区分。

## 书面摘要
height(身高)/avg（击球率）：同等身高，左手击球率较高，双手击球率偏向于中等，而低击球率的部分则是使用右手的球员分布较多。
weight(体重）/avg(击球率）：同等体重，高击球率部分左右手差异不明显，而低击球率部分则是使用右手的球员分布较多。
height(身高）/hr(全垒得分）：整体观察，获得全垒得分中，使用右手击球的球员较多。
weight(体重）/hr(全垒得分）：整体观察，获得全垒得分中，使用右手击球的球员较多。

## 问题记录与改进

### 1、初始文件只有avg-height，过于单调
改进方法：增加了avg-weight选项，并增加可供人选择的按钮。

### 2、增加新选项之后，选择后会出现与原有图形重合
针对此问题，未能找到解决方法，由于该项目是用dimple.js完成，未找到相应方法去除原来所画图像，只能依赖手动刷新。

### 3、选择不同选项后，无提示
改进方法：增加了选择选项后，选项div的属性变化。

### 4、图中的缩写字母含义不明确
改进方法：为缩写字母添加文字说明。

# 20180506更新文件index_v2.html
## 说明：
该文件主要针对原有问题2做了修复，主要用了d3.js方法完成该项目。

# 20180507更新文件index_v3.html
## 说明：
该文件主要针对问题4，对图中缩写添加了文字说明。
