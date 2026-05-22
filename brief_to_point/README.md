# Claude Code Skill: brief_to_point

一个为 Claude Code 打造的「言简意赅」效率插件。彻底消除 AI 在复杂技术对话中对同一点反复揉碎、车轱辘话带来的信息冗余，在大幅节省 Token 的同时，保持极高的专业解答质量。

## 核心特性
- **高密度输出**：单点结论绝不重复描述，直击要害。
- **质量不妥协**：深度技术细节与逻辑推导百分之百保留。
- **工具安全**：默认开启高效读取权限（`cat`/`awk`/`grep` 等），写操作强制执行前置二次确认。

## 安装方法

通过 Claude Code 的命令行工具或软链接直接加载：

```bash
# 方式 A：克隆到你本地的项目配置目录（推荐）
cd /path/to/your/project
mkdir -p .claude/skills
git clone [https://github.com/你的用户名/brief_to_point.git](https://github.com/你的用户名/brief_to_point.git) .claude/skills/brief_to_point

# 方式 B：全局软链接安装
git clone [https://github.com/你的用户名/brief_to_point.git](https://github.com/你的用户名/brief_to_point.git) ~/.claude/skills/brief_to_point
