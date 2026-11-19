# 缩略散点图插件使用指南

## 一、使用步骤

### 步骤一：登录 DataEase 系统

打开浏览器，访问 DataEase 系统并完成登录。

### 步骤二：上传插件

上传插件（插件：scat-backend-2.10.22.jar，可联系管理员获取插件），若插件已经上传，无需重新上传。

<img src ="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img.png" alt="上传插件">

上传插件后需重启 DataEase 服务，进入部署 DataEase 所在服务器的后台，执行以下命令：

```bash
docker restart dataease
```

### 步骤三：创建视图

创建仪表板/数据大屏，选择缩略散点图。


<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img2.png" alt="创建视图">

### 步骤四：准备数据

选择数据集，并配置维度数据。

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img3%282%29.png" alt="准备数据" />

缩略散点图的本质，是在二维平面上，以点为载体，同时展示「类别 / 维度、两个数值指标（X/Y 轴）、可选的气泡大小 / 颜色指标」的多维度数据分布可视化工具，它的核心逻辑是通过点和对应的属性数据来传递信息，更侧重于二维指标的关联与分布展示。

字段说明:

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img4.png" alt="字段说明">



***注意:如果横轴 / 纵轴的数值字段存在 NULL、空字符串，会导致图表加载失败。***

数据示例：

| 统计年度 | 行业 | 总资产周转率 |   净利率   |
|------|----|--------|------|
| 1998 | 公路与铁路  | 0.2266 | 0.4201 |
| 1998 |农产品| 0.8537 | 0.2064 |
| 1998 | 出版  | 0.315  | 0.0986 |
| 1998 | 制药  | 0.7548 | 0.2626 |
| 1998 | 包装食品与肉类  | 1.2637 | 0.1303 |
| 1998 | 化肥与农用药剂  | 0.5709 | 0.188 |
| 1998 | 商品化工  | 1.0309 | 0.2125 |
| 1998 | 啤酒酿造商  | 0.4103 | 0.1791 |
| 1998 | 复合型公用事业  | 0.3577 | 0.1344 |
| 1998 | 多种化学制品  | 0.4077 | 0.237 |
| 1998 | 多种金属与采矿  | 0.7984 | 0.1076 |

基于以上数据创建数据集：

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img5.png" alt="数据集图片" />

## 二、样式配置

### 1. 标题样式

配置图表标题的样式属性。

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img6.png" alt="标题样式" />

### 2. 基础样式

基础样式支持配置以下内容：

**配色方案：**支持选择预设的配色方案，按数据分组的顺序为散点依次分配颜色

**不透明度：**调整散点节点颜色的不透明度（0-100%）

**图形形状：**支持切换散点的展示形状，可选圆形、矩形、三角形、菱形等

**节点大小：**设置散点节点的尺寸大小；当数据点数量较多时，建议调小尺寸以避免重叠遮挡

**标签显示：**控制散点标签的开关状态，可自定义是否显示维度字段的名称

**提示框：**控制鼠标悬浮时提示框的开关状态，用于展示该数据点的完整维度与指标信息

**坐标轴样式：**支持配置坐标轴的显示状态、刻度、标签等样式

注意:不建议勾选「单一配色」，否则所有散点颜色一致，无法通过颜色区分不同类别数据。推荐使用预设配色方案，按分组顺序自动分配颜色，提升数据辨识度。

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img7.png" alt="基础样式">

### 3. 背景样式

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img8.png" alt="背景样式">

支持更换背景颜色,可以定义上传图片作为背景,也可以更换边框

### 4. 标签样式

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img9%282%29.png" alt="标签样式">



可以设置标签的颜色

### 5. 提示样式

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img10.png" alt="提示样式">

可以更换背景颜色和十字准线颜色,更改缩略半径

### 6. 横轴与纵轴样式

<img src="https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scat/img11.png" alt="横轴与纵轴样式">

支持显示轴名称,轴值可以修改为自动值,轴线可以改为实线,虚线和点,可以显示网格线







