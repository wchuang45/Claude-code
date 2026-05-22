# Claude-code
```markdown

Claude Code 安装流程及自定义 Skill 配置指南

## 环境准备

### 安装 Node.js

```bash
conda install anaconda::nodejs
```

### 配置 Node.js

```bash
mkdir ~/.npm-global
npm config set prefix '~/.npm-global'
echo 'export PATH=~/.npm-global/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
```

### 安装 Claude Code

Node.js 安装完成后，即可安装 Claude Code：

```bash
npm install -g @anthropic-ai/claude-code@latest
```

### 初始化配置

运行以下命令开始配置 Claude，选择中文/英文版本即可：

```bash
npx @z_ai/coding-helper
```

配置完成后，使用以下命令启动：

```bash
claude
```

## 配置文件

### 配置文件路径

```bash
vim ~/.claude/settings.json
```

### 配置示例（以智谱 GLM 为例）

```json
{
  "env": {
    "ANTHROPIC_AUTH_TOKEN": "API_KEY",
    "ANTHROPIC_DEFAULT_HAIKU_MODEL": "GLM-5-Turbo",
    "ANTHROPIC_DEFAULT_SONNET_MODEL": "GLM-5-Turbo",
    "ANTHROPIC_DEFAULT_OPUS_MODEL": "GLM-5-Turbo",
    "ANTHROPIC_BASE_URL": "https://open.bigmodel.cn/api/anthropic",
    "API_TIMEOUT_MS": "3000000",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1"
  }
}
```

## 注意事项

- 请将配置文件中的 `API_KEY` 替换为您的实际 API 密钥
- 根据实际使用的模型服务商调整 `ANTHROPIC_BASE_URL` 和模型名称
- 超时时间可根据网络情况适当调整
```
