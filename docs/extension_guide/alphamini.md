# 悟空机器人(教育版)
![](https://assets-new.ubtrobot.com/pc/static/cn/images/alphamini_v2/banner.jpg)


# 使用说明
目前该插件并未内置到 Adapter 中。

我们目前将插件构建为 [Adapter Node](https://adapter.codelab.club/dev_guide/Adapter-Node/)，可以在Adapter外部以普通Python文件运行，一旦运行起来，与普通Adapter插件是一样的，能够与Adapter体系的所有事物交互。

## Python环境
首先你本地需要有 Python 环境（`Python>=3.6`）

你可以到 [Python 官方](https://www.python.org/)下载，也可以使用 CodeLab放在[国内的版本(Python3.7)](https://www.codelab.club/blog/2020/08/20/tools#python)

!!! 提醒
    Mac 用户和 Linux 本地很可能内置了 Python3

### 安装依赖
```bash
pip install alphamini codelab_adapter_client --upgrade 
```

## 开始！


### 步骤 1：打开 [CodeLab Scratch](https://scratch-beta.codelab.club)
运行CodeLab Adapter， 确保在线平台与Adapte连接正常。

看到 [CodeLab Scratch](https://scratch-beta.codelab.club) 指示灯显示绿色，代表连接成功。

![](/img/v2/codelab-scratch3.png)

<!--
下载 [CodeLab Scratch Desktop(离线版)](https://www-old.codelab.club/blog/2020/08/20/tools/)，并运行它。

![](../img/scratch3-home.png)
-->
### 步骤 1：运行 node_alphamini.py

将  [node_alphamini.py](https://github.com/CodeLabClub/codelab_adapter_extensions/blob/master/nodes_v3/node_alphamini.py) 插件下载到本地（随便放在一个文件夹里），在命令行中进入到这个文件夹，使用 `python node_alphamini.py` 运行它。

### 步骤 2：为 悟空机器人 配网

将 悟空机器人 连上网络。（操作细节可以参考 悟空机器人 说明书）


### 步骤 3: 编程

选择 scratch3 中的 EIM 插件.

[alphamini-demo2](https://scratch-beta.codelab.club/?sb3url=https://adapter.codelab.club/sb3/alphamini-demo2.sb3)

以上 Demo 运行结果为: 

<video width=80% src="/video/1600057226116780.mp4#t=0.001" controls="controls"></video>

<!--<img width="600px" src="/img/scratch3_tello.png"/>-->

<!--
以下是一个简单 demo: 

![](/img/d5f48154f5c40003eeb416137b1055ad.png)


[tello3-demo](https://scratch-beta.codelab.club/?sb3url=https://adapter.codelab.club/sb3/tello3-demo.sb3)
-->

<!--![](/img/870f31bff87dc33c9640280c786ca483.png)-->

<!--<img width="600px" src="/img/46f87c6602288de4df896243fc87a3dc.png"/>-->


# 进阶

更多API参考文档: [mini-python-sdk](https://web.ubtrobot.com/mini-python-sdk/guide.html)




## 悟空的[内置行为](https://web.ubtrobot.com/mini-python-sdk/additional.html)

### [内置舞蹈](https://web.ubtrobot.com/mini-python-sdk/additional.html#id2)
```python
robot.play_behavior(name='custom_0035')  # 生日快乐
```

### [内置动作](https://web.ubtrobot.com/mini-python-sdk/additional.html#id3)
```python
robot.play_action(action_name='010') # 打招呼
```

### [内置表情](https://web.ubtrobot.com/mini-python-sdk/additional.html#id4)
```python
robot.play_expression(express_name='codemao13') # 疑问
```


---

!!! 提醒
    悟空内部运行一个安卓系统，带有内嵌 Python 环境