# Claude Code Skill: brief_to_point

一个为 Claude Code 打造的「言简意赅」效率插件。彻底消除 AI 在复杂技术对话中对同一点反复揉碎、车轱辘话带来的信息冗余，在大幅节省 Token 的同时，保持极高的专业解答质量。

## 核心特性
- **高密度输出**：单点结论绝不重复描述，直击要害。
- **质量不妥协**：深度技术细节与逻辑推导百分之百保留。
- **工具安全**：默认开启高效读取权限（`cat`/`awk`/`grep` 等），写操作强制执行前置二次确认。

## 安装方法

请在终端中复制并运行以下一键安装命令，即可将该技能直接部署到 Claude Code 的全局技能目录中：

```bash
# 1. 创建并进入目标技能目录
mkdir -p ~/.claude/skills/brief_to_point && cd ~/.claude/skills/brief_to_point

# 2. 将该仓库下的skill.json和README.md拷贝到 ~/.claude/skills/brief_to_point文件夹下即可
# 3. 启动claude，输入：帮我激活一下~/.claude/skills/brief_to_point这个skill即可
# 4. 重启claude生效skill


