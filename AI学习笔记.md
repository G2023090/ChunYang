# AI学习笔记

1. LLM 大语言模型（内部架构为transformer）

2. Token  大模型处理数据的最基本单元  

   1. 分编码解码，大模型一个token一个token接受输入再一个token一个token输出
   2. 词和token没有一一对应的关系，是模型自己的一套划分规则。

3. Context  上下文

   1.  包括对话历史和用户问题等

4. Context Window 大模型的Context最多能够储存的Token量

5. Prompt 提示词 

   1. 要清楚一点，让AI可以明白需要做什么
   2. Use Prompt：具体任务，由用户输入
   3. System Prompt: 人设和做事规则，由开发者后台配置好

6. Tool 工具，函数


7. MCP   统一工具接入标准，开发者只用按一个标准做工具

8. Agent 能自主规划自主调用工具，直至完成用户任务的系统

9. Agent Skill 给agent看的说明文档，不同agent的具体操作可能不同

   1. 按需加载，在根据描述找到对应的SKILL之后再打开.md文件

   2. Reference 按需中的按需，XXX.md文件和SKILL.md文件同级，并且要在SKILL.md文件里加入“仅在提到XXX的时候触发。需要读取XXX.md，然后XXX”

   3. Script 只会执行不会读取


   4. MCP 和Agent Skill
      MCP给大模型提供数据，本质程序
      Agent Skill教大数据如何处理数据，本质文档