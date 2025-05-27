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

#### 部署故障排除

如果遇到依赖安装错误，请确保：
- 使用了优化后的 `requirements.txt` 文件（包含版本范围而非固定版本）
- `runtime.txt` 指定了Python 3.11版本
- `packages.txt` 包含了必要的系统依赖

常见问题解决：
- **tiktoken编译错误**: 已在requirements.txt中使用兼容版本范围
- **Python版本不兼容**: runtime.txt指定使用Python 3.11
- **依赖冲突**: 使用灵活的版本范围避免严格锁定

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

## 配置文件说明

- `requirements.txt`: Python依赖包（使用版本范围确保兼容性）
- `runtime.txt`: 指定Python版本为3.11
- `packages.txt`: 系统级依赖包
- `.streamlit/config.toml`: Streamlit应用配置

## 注意事项

- 需要有效的OpenAI API密钥
- 支持的文件格式：PDF
- 建议上传的PDF文件大小不超过10MB
- 部署时会自动安装所有必要依赖

## 许可证

MIT License 