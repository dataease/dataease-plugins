# 散点连线图插件使用指南

## 一、使用步骤

### 步骤一：登录 DataEase 系统

打开浏览器，访问 DataEase 系统并完成登录。

### 步骤二：上传插件

进入系统设置页面，点击左侧菜单中的 **插件管理**，在图表插件列表中上传散点连线图插件。若插件已经上传，无需重新上传。

![截图1](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE1.png)

上传插件后需重启 DataEase 服务，进入部署 DataEase 所在服务器的后台，执行以下命令：

```bash
docker restart dataease
```

### 步骤三：选择散点连线图

在仪表板/数据大屏配置页面，先在左侧图表分类中选择 **关系** 类别，然后找到并点击 **散点连线图** 图标。

![截图2](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE2.png)

### 步骤四：准备数据

选择散点连线图所使用的数据集，然后将需要的字段分别拖入对应的维度和度量区域中。

![截图3](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE3.png)

## 二、样式配置

### 1、标题样式

可配置图表标题的文本内容、字体、字号、加粗/斜体/下划线、对齐方式、字体颜色、字体描边、显示备注等样式属性。

![截图4](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE4.png)

### 2、基础样式

基础样式支持配置以下内容：

- **配色方案**：选择图表的配色方案
- **不透明度**：图表颜色的不透明度
- **柱宽**：线条的宽度
- **点大小**：散点的大小
- **圆形**：数据点的形状
- **平滑线**：是否将连接线显示为平滑曲线
- **数据标签**：是否在数据点上显示数值标签
- **标题**：是否显示图表标题
- **坐标轴**：是否显示坐标轴
- **网格**：是否显示网格线
- **图例**：是否显示图例

![截图5](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE5.png)

### 3、背景样式

支持配置视图的内边距、圆角、背景模糊、背景颜色、背景图片、背景边框等样式属性。

![截图6](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE6.png)

### 4、标签属性样式

可设置数据点标签的样式属性：

- **标签**：控制数据点标签的显示/隐藏
- **全量显示**：是否显示所有数据点的标签
- **文本颜色**：设置标签文本的颜色
- **字号**：设置标签文本的字体大小
- **位置**：设置标签的显示位置，支持上、下、左、右

![截图7](https://north-dataease-1251506367.cos.ap-beijing.myqcloud.com/apps-dataease/view-scatterline/%E6%88%AA%E5%9B%BE7.png)
