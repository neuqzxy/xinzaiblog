---
title: 快速做一个Chrome BI Bot
excerpt: "这是文章摘要 This is the excerpt of the post"
---
{% note info  %}
本篇文章部分内容基于AI工具生成
{% endnote %}
# 什么是BI
BI 指的是商业智能(Business Intelligence)。它是一种帮助企业更好地理解和分析自身数据,从而做出更明智决策的技术和实践。主要包括以下几个方面:

数据收集和集成: 从各种源头(如 ERP、CRM 系统等)收集和整合企业内部和外部的数据。
数据分析和可视化: 利用报表、仪表板、图表等形式对数据进行分析和可视化展示,帮助用户洞察数据背后的趋势和洞察。
预测和建议: 利用高级分析技术(如机器学习、预测分析等)对未来趋势进行预测,并为决策提供建议。
支持决策: 将分析结果有效地传达给管理层,支持他们做出更明智的业务决策。
BI 系统通常涉及数据仓库、OLAP、报表、dashboards 等多个技术组件。其目标是帮助企业更好地理解自身的业务状况,发现问题并制定相应的策略,提高整体的竞争力和盈利能力。许多知名 BI 平台包括 Power BI、Tableau、Qlik Sense 等。

# 需要什么工作
我们会实现一个基于Chrome浏览器的BI Bot，实现鼠标选中一段文字，自动进行BI分析通过可视化的形式进行数据分析。分析需求，我们需要：
1. 一个Chrome 插件来完成对网页文字的选择记录
2. 选择一个合适的大语言模型
3. 编写prompt，使用大模型对选中文本进行BI分析
4. 使用合适的方式生成图表

# 站在巨人的肩膀上
不必重复造轮子，我们将选择业界成熟的工具完成我们的项目
1. 选择一个[chrome-extension-typescript-starter](https://github.com/chibat/chrome-extension-typescript-starter)，用来编写我们的Chrome Extension
2. 选择[VChart](https://visactor.io/vchart)作为我们的图表库
3. 选择[coze](https://www.coze.com/)作为机器人背后的大语言模型
4. 选择[VMind](https://visactor.io/vmind)进行图表推荐

## Coze



## 选择文本

## 提取数据
首先我们需要从指定的这段文字中提取出其中的数据内容，整理成一张表格，可以编写prompt如下：

> 从下面这段话中提取出有用的数据，生成csv，csv需要包含指标列数据列（数据列可以是多列），百分比需要转换为对应的小数，并且数据需要是准确的数字，，否则就过滤掉：

## 生成图表
## VMind
## VChart

## 展示
