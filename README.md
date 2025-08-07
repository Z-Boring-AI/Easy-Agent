# Easy Agent
一个简单的agent框架，使用function_calling的方式调用MCP工具

# 工具列表
目前提供以下工具
1. 计算器：用于计算公式
   使用示例
   ```
   Query:计算5*46+3
   结果：233
   ```
2. 天气查询：查询所在地的天气
   使用示例
   ```
   Query:广州的天气
   结果：晴，25℃，3级风
   ```
3. 文档写入：通过操控键盘实现内容的模拟输入
4. 打开文档软件：通过操控鼠标移动来打开文档软件 (通常与文档写入工具配合使用)
   使用示例
   ```
   Query:打开文档并输入hello world
   ```
5. 打开网页搜索内容：通过操控鼠标和键盘实现自动打开网页并输入搜索内容
   使用示例
   ```
   Query:搜索今天的新闻
   ```


# Quick Start
一、使用豆包作为LLM

1. 申请豆包API

   参考https://www.volcengine.com/docs/82379/1541594
2. 运行如下命令
```
  python -m mcp_tool.py mcp_client.py
```

二、使用GPT作为LLM
1. 申请openai的api key(需要包括api key、api version、endpoint)
2. 运行如下命令
   ```
   python -m mcp_tool.py mcp_client_gpt.py
   ```



