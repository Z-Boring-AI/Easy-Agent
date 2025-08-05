# Easy Agent
一个简单的agent框架，使用function_calling的方式调用MCP工具

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

# 运行示例
```[08/05/25 11:36:55] INFO     Starting MCP server 'agent_tool' with transport 'stdio'                                                                                                           

Connected to server with tools: ['weather', 'calculator', 'doc writer']

MCP Client Started!
Type your queries or 'q' to exit.

Query:计算5*46+3
工具calculator调用结果：233


Query:查询天气
工具weather调用结果：北京天气：
晴，25℃，3级风


Query:生成一个故事并保存到文档
工具doc writer调用结果：文档已保存为 agent_mcp.docx
```

