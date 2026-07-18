# save-to-learn

一个长期使用的学习素材库与 Codex skill，用于把网上或本地发现的好内容整理成可追溯、可分析、可检索、可复用的学习资产。

## 在线展示

素材库页面会展示已收录素材、标签、推荐程度和分析报告，并支持搜索与分类筛选：

**[打开学习素材库](https://feng082.github.io/save-to-learn/)**

> 当前仓库属于 `feng082` 账号，因此 GitHub Pages 的项目地址是 `feng082.github.io/save-to-learn/`。`save-to-learn.github.io` 这种根域名需要名为 `save-to-learn` 的 GitHub 账号或组织才能使用。

## 这个项目包含什么

- `index.html`：可点击的学习素材库展示页
- `reports/`：公开的素材研读与复盘报告
- `SKILL.md`：Codex 的 `save-to-learn` skill
- `agents/`：skill 的代理配置
- `.github/workflows/pages.yml`：自动部署 GitHub Pages

一个用于长期管理学习素材的 Codex skill。

它可以把网页、本地文件、图片、文章、PDF、视频、音频、GitHub 项目和软件工具，整理成可追溯、可分析、可检索、可复用的学习资产。

## 功能

- 保存网络素材的原始链接
- 保存本地文件的快捷方式或路径引用
- 生成素材研读报告
- 维护统一的素材索引
- 对图片建立 STYLE 视觉风格档案
- 检查重复素材
- 根据已有 STYLE 检索和复用视觉风格

## 命令

```text
/save-to-learn
/save-to-learn save
/save-to-learn inbox
/save-to-learn search <关键词>
/save-to-learn style <STYLE编号>
/save-to-learn find-style <关键词>
/save-to-learn index
```

说 `save` 时，除了本地收录，还会同步更新 HTML 素材页并提交、推送到 GitHub；如果只想保存在本地，请明确说“只保存本地”。

也支持自然语言，例如：

- 收录这个链接
- 分析并收录这张图片
- 收录这个本地视频
- 处理 inbox 里的新素材
- 找适合 AI 教程的信息图风格
- 参考 STYLE-001

## 素材库结构

```text
学习素材库/
├─ inbox/       # 临时入口
├─ sources/     # 原始链接、快捷方式和允许保留的素材
├─ reports/     # 研读报告和 STYLE 风格总结
├─ index.md     # 统一索引
└─ rules.md     # 使用规则
```

## 设计原则

- 不擅自下载完整网页、在线视频或网页中的全部图片
- 不复制、移动或修改本地大型原始文件
- 优先保存可追溯的原始入口
- 不虚构无法确认的作者、日期、内容和分析结论
- 相近图片优先复用已有 STYLE 编号
- 默认先给出分析方案和提示词，不自动调用生图工具

## 安装

将本仓库复制到 Codex skills 目录：

```text
C:\Users\10167\.codex\skills\save-to-learn
```

安装后，在 Codex 中使用 `/save-to-learn` 或自然语言提交素材即可。
