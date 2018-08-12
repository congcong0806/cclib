[TOC]
## Markdown 的功能

### 标题

* 标题1
* 标题2
* 标题3
* 标题4
* 标题5
* 标题6
* 文本

### 加粗

**加粗的内容**

### 斜体字

*斜体的内容*

### 下划线

<u>下划线的内容</u>

### 文字色相

<span style="color:#2b9f46">文字色相的内容</span>

### 删除线

~~删除线的内容~~

### 画水平线

***
---
- - - -

### 引用块

>引用块的内容

### 无序列表

* 无序列表1
* 无序列表2
* 无序列表3

### 有序列表

1. 有序列表1
2. 有序列表2
3. 有序列表3

### 任务

* [ ] 任务1
* [ ] 任务2
* [x] 任务3

### 缩进

点击「缩进」缩进内容，也可以用快捷键 Tab 缩进内容

### 减少缩进

点击「减少缩进」减少缩进的内容，也可以用快捷键 Shift+Tab 减少缩进内容

### 插入链接

[印象笔记官网](https://www.yinxiang.co/)
印象大使：<https://www.yinxiang.com/community>
<a href="https://help.yinxiang.com/hc/zh-cn">印象笔记官方知识库</a>

### 插入图片

![使用印象笔记 管理你的第二大脑](http://ww1.sinaimg.cn/large/9b84e6acgy1fu3rbshozhj20s60bsnpd.jpg)

<img src="https://public-cdn.mokahr.com/72bcee7e-aaa6-4fef-880b-349c8db212b6.png">

### 插入表格

| 序号 | 笔记 | 内容 | 时间 |
| --- | --- | --- | --- |
| 1 | note1 | contents1 | 2018-08-20 09:14:34 |
| 2 | note2 | contents2 | 2018-08-20 09:14:38 |
| 4 | note3 | contents3 | 2018-08-20 09:14:41 |

<table>
    <tr>
        <th>序号</th>
        <th>笔记</th>
        <th>内容</th>
        <th>时间</th>
    </tr>
    <tr>
        <th>1</th>
        <th>note1</th>
        <th>contents1</th>
        <th>2018-08-20 09:14:34</th>
    </tr>
    <tr>
        <th>2</th>
        <th>note2</th>
        <th>contents2</th>
        <th>2018-08-20 09:14:38</th>
    </tr>
    <tr>
        <th>3</th>
        <th>note3</th>
        <th>contents3</th>
        <th>2018-08-20 09:14:41</th>
    </tr>
</table>

### 添加图表

* pie chart（饼状图）
```chart
,Budget,Income,Expenses,Debt
June,5000,8000,4000,6000
July,3000,1000,4000,3000
Aug,5000,7000,6000,3000
Sep,7000,2000,3000,1000
Oct,6000,5000,4000,2000
Nov,4000,3000,5000,

type: pie
title: Monthly Revenue
x.title: Amount
y.title: Month
y.suffix: $
```

* line chart（线形图）
```chart
,Budget,Income,Expenses,Debt
June,5000,8000,4000,6000
July,3000,1000,4000,3000
Aug,5000,7000,6000,3000
Sep,7000,2000,3000,1000
Oct,6000,5000,4000,2000
Nov,4000,3000,5000,

type: line
title: Monthly Revenue
x.title: Amount
y.title: Month
y.suffix: $
```

* column chart（柱状图）
```chart
,Budget,Income,Expenses,Debt
June,5000,8000,4000,6000
July,3000,1000,4000,3000
Aug,5000,7000,6000,3000
Sep,7000,2000,3000,1000
Oct,6000,5000,4000,2000
Nov,4000,3000,5000,

type: column
title: Monthly Revenue
x.title: Amount
y.title: Month
y.suffix: $
```

* bar chart（条线图）
```chart
,Budget,Income,Expenses,Debt
June,5000,8000,4000,6000
July,3000,1000,4000,3000
Aug,5000,7000,6000,3000
Sep,7000,2000,3000,1000
Oct,6000,5000,4000,2000
Nov,4000,3000,5000,

type: bar
title: Monthly Revenue
x.title: Amount
y.title: Month
y.suffix: $
```

### 内嵌代码
`this is code`

### 插入代码块
```Java
public static void before() {
    try {
        Class.forName("org.sqlite.JDBC");
        c = DriverManager.getConnection("jdbc:sqlite:" + path);
        System.out.println("Opened database successfully");
        stmt = c.createStatement();
    } catch (Exception e) {
        e.printStackTrace();
    }
}
```
```ObjectiveC
#import <Foundation/Foundation.h>

int main(int argc, char *argv[]) {

    @autoreleasepool {
        NSLog(@"Hello World!");
    }

   return 0;
}
```
```Swift
var teamScore = 0
for score in individualScores {
    if score > 50 {
        teamScores += 3
    } else {
        teamScores += 1
    }
}
teamScore
```
``` Python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```

### 添加数学公式

支持 KaTeX 和 LaTeX 数学公式

```math
e^{i\pi} + 1 = 0
```

$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$

$x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

### 添加流程图

流程图（Flow Chart）：使用图形表示算法的思路是一种极好的方法，因为千言万语不如一张图。

```mermaid
graph TD
A[模块A] -->|A1| B(模块B)
B --> C{判断条件C}
C -->|条件C1| D[模块D]
C -->|条件C2| E[模块E]
C -->|条件C3| F[模块F]
```

### 添加时序图

时序图（Sequence Diagram），又名序列图、循序图，是一种UML交互图。它通过描述对象之间发送消息的时间顺序显示多个对象之间的动态协作。它可以表示用例的行为顺序，当执行一个用例行为时，其中的每条消息对应一个类操作或状态机中引起转换的触发事件。

```mermaid
sequenceDiagram
A->>B: 是否已收到消息？
B-->>A: 已收到消息
```

### 添加甘特图

甘特图（Gantt chart）又称为横道图、条状图(Bar chart)。其通过条状图来显示项目，进度，和其他时间相关的系统进展的内在关系随着时间进展的情况。

```mermaid
gantt
title 甘特图
dateFormat  YYYY-MM-DD
section 项目A
任务1           :a1, 2018-06-06, 30d
任务2     :after a1  , 20d
section 项目B
任务3      :2018-06-12  , 12d
任务4      : 24d
```

### 切换主题

* 白色
* 黑色
* 深空色
* 印象绿(大象定制)

### 编辑模式

可以切换编辑+预览双屏模式和纯编辑模式
    
### 支持HTML

<img src="https://www.yinxiang.com/media/img/market/market_lander_moleskine_d@2x.jpg" width=240>

<img src="https://public-cdn.mokahr.com/72bcee7e-aaa6-4fef-880b-349c8db212b6.png">

### 图床

暂不支持图床功能

