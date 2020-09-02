# Sparkify项目

本项目为*Udacity Nano Degree* 最终的实战通关项目，下方为项目相关文件和源码链接：

- [Github Repo](https://github.com/Novelan/Sparkify)
- [CSDN-Sparkify项目分享](https://blog.csdn.net/novelan/article/details/108325284)

```
##要使用此项目，请首先使用以下命令在你的设备上克隆repo

git init
git clone [链接]
```

- Sparkify项目技术分享博客：

## 项目简介

本项目使用***Spark***来分析探索某数字音乐服务平台***Sparkify***（类似于网易云音乐和QQ音乐的音乐平台）***2016年10月1日-2016年12月1日***期间用户在该平台上的行为数据。通过对用户行为和用户信息的探索性分析，提取提取可能对预测用户是否流失有帮助的相关特征，从而建立流失用户预测模型。

## 常用工具及使用版本

- numpy  --<1.16.5>
- pandas --<0.25.1>
- matplotlib.pyplot --<3.1.1>
- seaborn  --<0.9.0>
- pyspark --<3.0.0>

## 数据集
为了快速分析建模，该项目使用的是完整数据集（12GB）的迷你集`mini_sparkify_event_data.json`（128MB），分析完成后，再将项目整个流程部署到Amazon云。


## 数据属性
| 变量名称 | 所属类型 | 说明 |
| :- | :- | :- |
| artist | 音乐信息 | 歌手名称 |
| auth | 网页信息 | 用户进入平台的方式 |
| firstName | 用户信息 | 用户的名 |
| gender | 用户信息 | 用户性别：F为女，M为男 |
| itemInSession | 网页信息 | 会话顺序 |
| lastName | 用户信息 | 用户的姓氏 |
| length | 音乐信息 | 音乐时长（秒） |
| level | Event | 用户等级：free为免费用户，paid为付费用户 |
| location | 会话信息 | 用户在会话期间所属位置 |
| method | 网页信息 | HTTP method ,GET 或者 PUT |
| page | 网页信息 | 用户行为类型 |
| registration | 用户信息 | 用户注册时间 |
| sessionId | 会话信息 | 会话编号 |
| song | 音乐信息 | 歌曲名称 |
| status | 网页信息 | HTTP状态编码. 2xx=Successful, 3xx=Redirection, 4xx=Client Error. |
| ts | 网页信息 | 用户行为发生的时间 |
| userAgent | 会话信息 | 网络环境，所属浏览器 |
| userId | 用户信息 | 用户编码，具有唯一性 |

## 数据分析流程
- 评估和清理数据
- 探索性数据分析
    - 定义流失和留存
    - 分类探索流失和留存用户在各个变量上的数据分布（使用可视化工具，如matplotlib.pyplot, seaborn）
    - 提取可能对预测用户是否流失有帮助的相关特征
- 特征工程
- 建模
    - 拆分数据，将数据分成训练集，验证集和测试集
    - 数据预处理
    - 模型选择
    - 网格化调参
    - 评估结果
- 反思和总结


## 隐私
项目中的个人隐私信息，如姓名、具体地址将不用作主要分析


