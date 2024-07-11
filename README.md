# HighSchoolMathRAG
high school math RAG

## 计划

### 2024-07-09

<<<<<<< HEAD
- [ ] 环境搭建，
=======
- [x] 环境搭建，
>>>>>>> c041e8dd252d02936bcea46566418a847ef32634
  - [ ] 使用mini conda创建一个本地可调用 nvidia语言模型的环境
  - [ ] 使用 mini conda 将环境打包，并上传到本仓库
  - [ ] 群里已经有人提供requirements.txt 文件（已上传到本代码仓），可尝试安装环境
  - [ ] mini conda 参考资料：https://www.runoob.com/python-qt/anaconda-tutorial.html
<<<<<<< HEAD
- [ ] 材料收集，10篇高考数学题目及其答案
- [ ] 使用环境跑通一个调用nvidia 模型的最简单示例
  - [ ] 参考教程：回顾训练营第一二节，研究一下如何获取 key，本地配置key，调用模型
- [ ] 若环境搭建过程中，遇到问题，可在 大群里 @ 一下助教，或者问一下其他参赛者，将自己遇到的问题直接发在群里咨询
- [ ] 本地IDE环境，建议使用 VScode，并且安装 marscode 智能插件提升代码编写效率
=======
- [x] 材料收集，10篇高考数学题目及其答案
- [x] 使用环境跑通一个调用nvidia 模型的最简单示例
  - [x] 参考教程：回顾训练营第一二节，研究一下如何获取 key，本地配置key，调用模型
- [x] 若环境搭建过程中，遇到问题，可在 大群里 @ 一下助教，或者问一下其他参赛者，将自己遇到的问题直接发在群里咨询
- [x] 本地IDE环境，建议使用 VScode，并且安装 marscode 智能插件提升代码编写效率
>>>>>>> c041e8dd252d02936bcea46566418a847ef32634
  - [ ] marscode 智能插件参考链接：https://code.visualstudio.com/Download

### 2024-07-10

<<<<<<< HEAD
- [ ] 根据训练营中教程，启动服务，跑通最简单的包含前端的问答流程，搭建起一个最基本的环境
=======
- [ ] 更新：无需做中英互译，模型自带多语言功能
- [ ] **今日主要目标**： 基础bot上线，能够拿到完赛证明
- [ ] 根据 **目标** 章节 的描述，生成提示词
- [ ] 对收集的文档进行向量化，并保存到本地
- [ ] 根据训练营中教程，启动服务，跑通最简单的包含前端的问答流程，搭建起一个最基本的环境
  - [ ] 创建一个最简单的问答机器人
  - [ ] 判断标准：
    - [ ] 1。能够生成一个 界面进行交互
    - [ ] 2。能够对最近几年的高考数学题目进行提问和交互

### 2024-07-11

- [ ] 自由发挥

- [ ] 加分项

  | 加分项         | 难度 | 内容                           |      |
  | -------------- | ---- | ------------------------------ | ---- |
  | gradio界面美化 | *    | 做成二次元风格，添加背景图片等 |      |
  | 调用更多接口   | **   | 上传图片，并识别图片内容       |      |
  | 调用更多接口   | ***  | 使用语音交互，语音识别         |      |
  | 调用更多接口   | **** | 将生成的回答转换为语音并回复   |      |
  |                |      |                                |      |

  
>>>>>>> c041e8dd252d02936bcea46566418a847ef32634



## 前言

1. 以赛代练，通过比赛快速熟悉相关理论及其应用，获取感性认识
2. 能够快速实现想法，为后续科研/工作 培养能力

## 目标

1. 能够作为高中学生的私人数学指导老师

### 能力

1. 拥有30年以上高中数学教学经验
2. 获得特级教师以上资格证书
3. 对学生个人情况完全了解
4. 能够从学生的视角看待新的问题
5. 对每个题目都能给出3种以上的解题方法，并对每种解题方法的思路非常清晰
6. 能够快速分析出题目出题人的意图，指出出题人想要考察的知识点，设置的陷阱
7. 能够记录学生问过的所有题目，学生做错过的所有题目，并能够分析其做错的原因，然后从题库中给出相类似的题目

### 文档

1. 中国高考历年数学试卷（1978至2024）及其官方解答的  pdf 版本
   1. 全国乙卷、全国甲卷、新高考1卷(新课标1卷)、新高考Ⅱ卷(新课标Ⅱ卷)、自主命题卷
2. 五年高考，三年模拟
3. 黄冈名卷
4. 学而思，新东方，好未来 k12 培训机构 网课教材
5. 高中课本例题
6. 学生个人历次试卷（模拟学生真实场景）

### 实现

#### 相关技术

1. 图像识别：拍照上传题目，错题，解题过程等
2. 公式识别：数学中存在大量公式，需要特殊的公式识别能力
3. LLM：对题目进行分析，给出题解，对文档进行预处理，形成 vectors等（培训课程相关内容）
4. 翻译：英汉互译（模型大概率是使用英文预料进行预训练，因此需要一个英汉互译的转换过程）
5. 语音识别：对提问做出相应的回答。语音转文字，文字转语音。

#### 技术栈

1. 开发语言：Python
2. 开发平台：Nvidia 比赛环境
3. 知识储备：图像识别，LLM

#### 实现步骤

1. 收集相关 pdf 材料，构成后续知识库文档
2. 调研相关技术中需要使用的各种函数接口
   1. 语音识别是可选项，锦上添花，仅作为了解，

#### 操作步骤

1. 上传照片， 上传相关问题
2. 获取返回结果，返回结果可参考 demo.pptx 中对一个题目的解题方式及其分析。
3. 对返回结果进行追问

#### 后台服务

1. 图像识别
2. 公式识别
3. 知识库维护，更新

### 任务分工

1. 文档收集，资料清洗-饥饿，embrace
2. 知识库维护，LangChain流程设计-饥饿
3. 图像识别，公式识别-embrace
4. 服务设计-宣辰
5. 函数接口调研-SYL
6. 总体指导-WYT
7. 算法实现，落地-饥饿，embrace

备注：

1. 文档收集不需要花费太多时间，只需要能够验证流程即可，10篇pdf即可，耗时在半天以内
2. 任务分工中的 2，3 可讨论，根据两位兴趣进行选择，一个偏向LLM 方向，一个偏向 图像处理
3. 收集到的资料直接上传到本代码仓
4. 相关调试代码，直接上传到本代码仓
5. 若对 git 命令不熟，则快速学习一下 git相关命令，每人创建一个自己的分支，git 参考资料：https://www.runoob.com/git/git-basic-operations.html
6. github 参考资料：https://www.runoob.com/w3cnote/git-guide.html

