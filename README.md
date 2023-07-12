# LogiQuest:A Dataset for Free-Text Logical Reasoning and Inference

逻辑推理是人工智能的关键能力之一，特别是对于大模型如ChatGPT。为了提升其推理和理解能力，我们需要大量的逻辑和推理训练数据。然而，现有的训练数据通常集中于英语，对于中文的逻辑和推理训练数据，特别是那些涉及到具体和复杂问题的，供应十分匮乏。
为了解决这个问题，我们从互联网上收集了大量的逻辑推理对话数据，包含各种问题以及它们的答案。我们的目标是通过使用这些数据来训练GPT，以增强其逻辑推理和理解能力。
我们首先公开了1936条数据，称之为“LogiQuest-Dataset-V1”。

## 数据样例

### 例1
```json
{
  "system": "Assistant扮演一名对话机器人。User每次输入一个问题，Assistant做出相应回答。不使用任何插件。", 
  "source": "", 
  "language": "Chinese", 
  "user": "S先生：让我来猜你心中所想的字母，好吗? P先生：怎么猜?S先生：你先想好一个拼音字母，藏在心里。p先生：嗯，想好了。S先生：现在我要问你几个问题。P先生：好，请问吧。S先生：你所想的字母在CARTHORSE这个词中有吗? P先生:有的。S先生:在SENATORIAL这个词中有吗?P先生:没有。S先生:在INDETERMINABLES这个词中有吗? P先生:有的。S先生:在REALISATON这个词中有吗? P先生:有的。S先生:在ORCHESTRA这个词中有吗? P先生:没有。S先生:在DISESTABLISHMENTARIANISM中有吗？ P先生:有的。S先生:我知道，你的回答有些是谎话，不过没关系，但你得告诉我，你上面的六个回答，有几个是真实的? P先生:三个。S先生:行了，我已经知道你心中的字母是……。", 
  "assistant": "我感觉：应该是H", 
  "thought": "这是一个逻辑推理题目，需要通过分析和推理来找出答案。", 
  "title": "猜字母", 
  "command": "", 
  "plugin": ""
}
```

### 例2
```json
{
  "system": "Assistant扮演一名对话机器人。User每次输入一个问题，Assistant做出相应回答。不使用任何插件。", 
  "source": "", 
  "language": "Chinese", 
  "user": "95，88，71，61，50，（ ）     A、40；B、39；C、38；D、37；", 
  "assistant": "选A， 思路一：它们的十位是一个递减数字 9、8、7、6、5 只是少开始的4 所以选择A． 思路二： 95 - 9 - 5 = 81；88 - 8 - 8 = 72；71 - 7 - 1 = 63；61 - 6 - 1 = 54；50 - 5 - 0 = 45；40 - 4 - 0 = 36 ，构成等差数列", 
  "thought": "这是一个逻辑推理题目，需要通过分析和推理来找出答案。", 
  "title": "", 
  "command": "", 
  "plugin": ""
}
```

### 注：
1. 本次公开的数据（LogiQuest-Dataset-V1）包含中文和英文。对于其他语言，可以将我们公开的数据翻译成其他语言。
2. 本次公开的数据（LogiQuest-Dataset-V1）未经人工校验，无法严格保证正确性、安全性。使用者需要对数据产生的结果负责。

## 主要贡献者
1. 张琳, linzhang22@m.fudan.edu.cn
2. 李梓涵, zhli21@m.fudan.edu.cn
3. 熊卓帜, zzxiong21@m.fudan.edu.cn
4. 顾洲洪, zhgu22@m.fudan.edu.cn
5. 朱晓萱, xxzhu22@m.fudan.edu.cn 
6. 叶浩宁, hnye19@fudan.edu.cn
7. 王建宸, 20210240375@fudan.edu.cn
8. 蒋思航, tedsihangjiang@gmail.com
9. 冯红伟, hwfeng@fudan.edu.cn 
10. 肖仰华, shawyh@fudan.edu.cn 
11. 汪自力, ziliwang.do@gmail.com 
12. 王树森，wssatzju@gmail.com