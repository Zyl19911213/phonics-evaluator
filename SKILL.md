name: phonics-evaluator
description: 基于科大讯飞技术的智能英语发音纠错工具

Phonics Evaluator

基于科大讯飞技术的智能英语发音纠错工具。

功能描述

本 Skill 提供英语语音评测服务。用户提交一段英语文本及其对应的语音音频，系统会基于科大讯飞语音评测技术，对发音进行多维度打分，并返回总分及存在发音问题的单词列表。

使用方式

通过 API 或 MCP 调用 evaluate 工具，传入待评测文本和音频数据，即可获得评测结果。

输入参数

text (string, required): 待评测的英语文本

audio (string, required): 语音音频数据（Base64 编码）

输出结果

total_score (number): 发音总分（0-100）

problem_words (array): 存在发音问题的单词列表，每个元素包含单词文本及问题类型

API 端点

POST https://phonics-eval-iuhpfmedoi.cn-hangzhou.fcapp.run/api/evaluate
