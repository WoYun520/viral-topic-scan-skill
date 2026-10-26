# xhs-skill-viral-topic-scan

开源 Agent Skill：从公开社交与网页搜索抓取**高互动爆款选题**，去重写入本地《素材库.md》，并留下扫描日志。

- **只收集、不打扰**：不点赞、不评论、不收藏、不私信、不登录
- **不替你发帖**：素材留给人改编后再发
- **不绑死某一家 AI**：有搜索工具即可；Muse／Cursor／Claude／Codex 等只要能读本 `SKILL.md` 都能跑

作者：[Levi 卧云](https://x.com/zmdsb259414)（`@zmdsb259414`）

## 安装

### Cursor / Grok Bot 类

把本仓库放到 Agent 的 skills／workflows 目录，或复制 `SKILL.md` 为一条可加载 Skill。用下面启动话术触发。

### 通用（任何能读 Markdown 配方的助手）

1. Clone 本仓库到工作目录  
2. 把 `SKILL.md` 全文（或「启动话术」）发给助手  
3. 在同一工作目录下跑；产物是 `账号定位.md`、`素材库.md`、`scans/`

```bash
git clone https://github.com/WoYun520/xhs-skill-viral-topic-scan.git
cd viral-topic-scan
```

（仓库地址以 GitHub 实际名为准。）

## 启动话术

> 按 xhs-skill-viral-topic-scan Skill 跑一轮：先确认或写入账号定位，建好／读取《素材库.md》，搜索并去重后把新选题写入待用区，并在 scans/ 留下本轮日志。只收集，不互动、不发帖。

## 目录

| 路径 | 说明 |
| --- | --- |
| `SKILL.md` | Skill 正文（YAML frontmatter + 配方） |
| `examples/素材库.example.md` | 素材库模板 |
| `examples/账号定位.example.md` | 定位模板 |
| `LICENSE` | MIT |
| `VERSION` | 语义化版本 |

## 和「内容框架」的关系

本 Skill 只负责**看见高流量选题并入库**。主菜／添头、人机分工、发布权留给人——见你自己的内容框架；本仓库不内置发帖自动化。

## 许可

MIT。欢迎 Fork；二创请保留署名与许可证文件。
