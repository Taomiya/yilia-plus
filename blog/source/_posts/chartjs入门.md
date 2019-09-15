---
title: chartjs入门
date: 2019-09-12 10:48:09
tags:
  - 前端
  - chartjs
---
# chartjs #
**chartjs** 就是可以画各种图表的一款前端工具~

## 使用 ##
首先需要 char.min.js，点击下载[http://how2j.cn/frontdownload?bean.id=2097](http://how2j.cn/frontdownload?bean.id=2097)

在这边推荐一下一个网站，前端要引入的资源基本都可以在上面找到：
[https://www.bootcdn.cn](https://www.bootcdn.cn)

<!--more-->


### html代码

    <div style="width:400px;margin:0px auto">
    <canvas id="myChart" ></canvas>
    </div>

### js代码

通过 dom 操作获取 myChart 对象的 2d 上下文：
 

    var ctx = document.getElementById('myChart').getContext('2d');
 

1. 基于 ctx Chart对象，并传递如下参数进去
2. type: 'line' 表示这个是一个线型图表。 如果要柱状图，修改成 'bar' 就可以了
3. data: 提供要显示的数据
4.  labels 表示数据下方的文字： '红', '蓝', '黄', '绿', '紫', '橙'
5.  datasets 表示数据集合。 这里数据集合里只有一个数据，如果是多个数据，就会在图表上看到多条线，所以这里只会看到一条线。
6. label: 这组数据的名称
7. data: 具体数据
8. borderColor: 线条颜色
9. borderWidth: 线条宽度
10. fill: false. 不进行填充
11. options: 其他选项
12. tooltips 表示鼠标移动到图标的时候的提示信息。
13. intersect: false. 表示鼠标不放在数据点上时，也会显示提示信息。
14. model: 'index' 显示模式

``<script>
var ctx = document.getElementById('myChart').getContext('2d');
var myChart = new Chart(ctx, {
type: 'line',
data: {
labels: ['红', '蓝', '黄', '绿', '紫', '橙'],
datasets: [{
label: '示例',
data: [12, 19, 3, 5, 2, 3],
borderColor:'blue',
borderWidth: 1,
fill: false,
}]
},
options: {
tooltips: {
intersect: false,
mode: 'index'
}
}
});
</script>``
    
### 实现效果
![](https://i.imgur.com/ijBHjfh.png)：




