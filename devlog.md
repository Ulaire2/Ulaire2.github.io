# Devlog

个人主页的维护记录。按时间倒序，最新在上。

---

## 2026-04-12

- Gravity Flip 的 Windows 构建通过 GitHub Releases 发布（[Ulaire2/GravityFlip v0.1](https://github.com/Ulaire2/GravityFlip/releases/tag/v0.1)）。Gravity Flip 卡片的 `work-links` 从「Windows 构建 · 整理中」占位替换为实际的「下载 Windows 构建」按钮，`btn-outline` 样式。卡片顶部的 TODO 注释同步收敛到只剩「补一张封面图」。

---

## 2026-04-11

- 补了这份 `devlog.md`，从今天开始持续维护。
- 结构重构：新增「作品」板块（`#works`），独立的 `#tonecheck` 板块下线，ToneCheck 作为一张 work card 并入作品板块，与 Unity Demo 等其他作品并列展示。
- 清理了与被下线板块相关的 CSS（`.tonecheck-*`）和此前已注释掉的 ComfyUI 板块（HTML + `.comfyui-*` CSS）。
- 导航栏把 `ToneCheck 同调` 链接替换为 `Works 作品`，指向新的 `#works` 锚点。
- 作品板块第二张卡从占位更新为 Gravity Flip（Unity 6 + URP 做的 2.5D 精确平台跳跃 demo，设计核心是只有翻转重力一个能力 + 固定翻转次数约束）。填了标题「Gravity Flip」、描述、tags（`Unity 6` / `2.5D Platformer` / `学习项目`）。封面图暂缺，构建下载链接暂缺——`work-links` 里放了「Windows 构建 · 整理中」占位。

## 2026-03-30（项目初始搭建）

这一天完成了整个主页从零到可用的全过程，下面按大致顺序整理：

**初始化**
- `fc81655` / `64e70c0` / `eab10d6` 分批次上传初版文件。
- `966f96b` 删除旧版 `index.html`，`48dbf43` 将 `index2.0.html` 重命名为 `index.html`，完成主文件切换。
- `1a21205` / `b12e1ce` / `1de42d9` 处理 `images/` 目录下的占位文件和素材上传。

**结构搭建**
- `94c0e0c` / `c0e797c` / `2706f6c` 连续三次 Update index.html，完成骨架搭建。
- `228a12f` 建立 `resume/` 目录，用于放置简历 PDF。

**内容迭代**
- `13e3a63` 优化文件逻辑，迭代 index。
- `0f13d75` 继续迭代 index。
- `e9ffbd2` 优化 index。
- `965f186` 修改简历功能（双版本简历下载：游戏方向 / 通用方向）。
- `c783c86` 大改 landing 界面。
- `25f4cd5` 微调字体。
- `8e7c352` 继续修改。
- `7e26079` claude 迭代 index。

**收尾与隐藏**
- `55d58ef` 修改邮箱 cdn-cgi 混淆相关问题。
- `a054052` 暂时隐藏 AI 生图板块（ComfyUI 作品展示）。
- `d051271` 暂时隐藏 landing 导航栏，以及顶部的 AI 部分（hero-nav）。
- `c709c15` 更新简历。
- `cecf2e1` 加 favicon。
