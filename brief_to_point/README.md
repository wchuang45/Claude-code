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

# 2. 初始化 Git 并关联远程仓库
git init
git remote add origin [https://github.com/wchuang45/Claude-code.git](https://github.com/wchuang45/Claude-code.git)

# 3. 开启稀疏检出，配置仅下载 brief_to_point 文件夹内的内容
git config core.sparseCheckout true
git sparse-checkout set --no-cone "brief_to_point/*"

# 4. 拉取代码并将子文件夹内的文件直接释放到当前目录
git pull origin main --depth=1
mv brief_to_point/* ./ && rm -rf brief_to_point


