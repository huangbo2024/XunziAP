# 简介

本脚本基于[荀子大模型](https://github.com/Xunzi-LLM-of-Chinese-classics/XunziALLM), 一键快速完成给定古籍文本（txt/doc/docx）的断句和标点并保存为txt格式。

## 功能描述

- 读取`.txt`或`.docx`文件中的文本。
- 使用预训练的荀子大模型对文本进行处理，如添加标点、校正语法等。
- 将处理后的文本输出到新的文件中，文件名包含处理时间戳。

## 安装指南

   - 小白：注册并登陆[魔搭平台](https://modelscope.cn/models/Xunzillm4cc/Xunzi-Qwen-Chat/summary)后点右上角“NoteBook快速开发，选择由魔搭平台提供的免费PAI-DSW实例。
   - 进阶：自行选择平台部署。

## 使用方法
1. **安装依赖**
   - 在terminal上安装必要的Python库：
     ```
     pip install -r python-docx
     ```
2. **准备文件**
   - 上传`XunziAP.ipynb`至根目录。
   - 上传需要处理的`.txt`或`.docx`至根目录。

3. **运行脚本**
  - 点击`run`按钮执行脚本.

4. **检查输出**
   - 处理完成后，查看输出文件。输出文件位于同一目录下，文件名如`output_20220422_215135.txt`。

## 常见问题解答

**Q: 如何查看程序是否正确执行？**
A: 程序运行时会在控制台输出进度和结果，也可以查看服务器的日志文件。

**Q: 本脚本是否可以实现其他功能？**
A: 基于该大模型的基本原理，通过修改代码`input_text = '请对冒号后的话正确添加标点符号（断句），如果不需要就直接回复原文：' + para`中的prompt即可指定脚本实现其他功能，如翻译、分词等。

---

受朋友委托开发此脚本，希望能够帮助相关从业者进一步挖掘中国传统文化的丰富内涵。
