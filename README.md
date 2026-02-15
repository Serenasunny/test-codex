# test-codex

## 安装 virattt/dexter 到 ChatGPT（Codex Skills）

已尝试在当前环境直接联网安装 `https://github.com/virattt/dexter`，但网络代理返回 `403`，无法从 GitHub 拉取仓库。

你可以在本地终端运行下面命令完成安装：

```bash
python3 /opt/codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo virattt/dexter \
  --path .
```

如果仓库根目录不是一个可安装的 Skill（缺少 `SKILL.md`），请改为指定实际 skill 子目录：

```bash
python3 /opt/codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo virattt/dexter \
  --path <path/to/skill>
```

安装完成后：

1. 重启 ChatGPT/Codex 客户端会话。
2. 在新会话中验证技能是否可用。

> 提示：如果你愿意，我可以继续帮你判断 `dexter` 仓库里哪个目录才是正确的 skill 路径。
