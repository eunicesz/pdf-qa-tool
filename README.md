# 📑 AI智能PDF问答工具

这是一个基于Streamlit和LangChain构建的智能PDF问答工具，可以让用户上传PDF文件并对其内容进行智能问答。

## 功能特点

- 📄 支持PDF文件上传
- 🤖 基于OpenAI GPT-3.5-turbo的智能问答
- 💬 对话历史记录
- 🔍 文档检索和相关性匹配
- 🌐 简洁美观的Web界面

## 技术栈

- **前端框架**: Streamlit
- **AI模型**: OpenAI GPT-3.5-turbo
- **文档处理**: LangChain + PyPDF
- **向量存储**: FAISS
- **文本分割**: RecursiveCharacterTextSplitter

## 部署说明

### 在Streamlit Cloud上部署

1. Fork这个仓库到你的GitHub账户
2. 访问 [Streamlit Cloud](https://streamlit.io/cloud)
3. 连接你的GitHub账户
4. 选择这个仓库进行部署
5. 设置主文件为 `main.py`
6. 点击部署

### 本地运行

1. 克隆仓库：
```bash
git clone https://github.com/eunicesz/pdf-qa-tool.git
cd pdf-qa-tool
```

2. 安装依赖：
```bash
pip install -r requirements.txt
```

3. 运行应用：
```bash
streamlit run main.py
```

## 使用方法

1. 在侧边栏输入你的OpenAI API密钥
2. 上传PDF文件
3. 在文本框中输入你的问题
4. 等待AI生成答案
5. 查看历史对话记录

## 注意事项

- 需要有效的OpenAI API密钥
- 支持的文件格式：PDF
- 建议上传的PDF文件大小不超过10MB

## 许可证

MIT License 