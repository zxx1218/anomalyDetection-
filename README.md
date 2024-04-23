# 计算机毕业设计--基于深度学习的视频异常检测算法设计与实现

**我的CSDN中还有其他方向的深度学习毕业设计项目，例如车道线检测、图像破损修复，照片色彩增强，划痕检测、车牌识别、目标检测等，具体参考**
[深度学习方向毕业设计](https://blog.csdn.net/qq_45566099/category_12507289.html)

## :sparkles: 效果展示！

[video(video-lUdRnvMX-1713865282687)(type-csdn)(url-https://live.csdn.net/v/embed/381608)(image-https://live-file.csdnimg.cn/release/live/file/1713864551052.png?x-oss-process=image/resize,l_300)(title-异常检测Web演示视频)]


<hr>

#### 介绍
&emsp;&emsp;基于自编码器(AE)的帧重构(当前或未来帧)是一种流行的视频异常检测方法。在正常数据上训练的模型，异常场景的重建误差通常比正常场景大得多。以前的方法将记忆库引入AE，用于在训练视频中编码不同的正常模式。然而，这些方法过于消耗内存，无法处理测试数据中未见过的新场景。在这项工作中，本项目提出了一个动态单元来实时地将正常的视频动态进行编码，而不需要额外的内存开销。此外，本项目将元学习引入到模型中，形成了一个可通过少量学习即可快速适应各种现实视频场景的模型，称为元学习模块。该模块只需要几次更新迭代即可实现对新场景的快速适应能力。

#### 运行要求
- 算法需要在安装了Nvidia GPU和CUDA的计算机上运行，运行代码需要Python>=3.6
- 前后端页面需要Python>=3.6

## :rocket: 使用方式
- **giuhub链接：**[Github视频异常检测](https://github.com/zxx1218/anomalyDetection)

- **gitee链接：**[Gitee视频异常检测](https://gitee.com/zxx1218/anomaly-detection)

<hr>

## 通过运行算法源代码获取检测结果
clone项目后，只需一个简单的命令即可实现视频的异常事件检测（to/your/xxx.pth是你预训练模型的存放位置）

```
python Test.py --model_dir to/your/xxx.pth
```

## 通过部署Web端网页服务
cd到代码根目录下的gradioDemo文件夹下，然后执行python脚本（需要提前安装gradio包）
```
# 安装gradio包
pip install gradio 
# 启动Web服务
python gradio_demo.py
```
回车后会自动启动Web服务,默认启动端口为9091，在浏览器输入http://127.0.0.1:9091即可访问，在控制台看到如下信息代表成功启动👇
![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/c1a73a1a7d1f4f0091ec35b5215070c1.png#pic_center)
打开http://127.0.0.1:9091，显示如下界面👇
![在这里插入图片描述](https://img-blog.csdnimg.cn/direct/8986e1b9607f485bbcf18e30a7f81abe.png#pic_center)



## 通过搭建前后端Web页面实现视频上传与自动检测

- **Web端体验地址：（稍后部署后更新）**

<hr>

## :pencil2:	如何自行训练模型?

- **咨询作者**

## 有问题联系作者：
- VX：Accddvva
- QQ：1144968929
- 该项目在github与gitee上提供训练好的模型文件以及调用该文件的测试代码，clone后安装环境即可使用
- **本项目完整代码（测试+训练+模型定义）+ 环境配置教程 + 代码使用方式 ==> 价格300RMB，可提供远程部署服务，另外没有合适的显卡的同学可提供GPU服务器短期租赁服务，24G显存服务器每个月100RMB**

<hr>

#### :fire:广告
- 作者于浙江某985高校就读人工智能方向研究生，可以帮忙定制设计模型，并提供源代码和训练后的模型文件以及环境配置和使用方法，只需要描述需求即可。
- 人工智能领域，尤其是计算机视觉（Computer vision，CV）方向的毕业设计，只要你想得出，没有做不出的
