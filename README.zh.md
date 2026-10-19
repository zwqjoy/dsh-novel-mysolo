# dsh-novel-mysolo

面向 DeepSeek Harness 的单代理小说创作插件，提供 `novel-mysolo` 预设，显示名称为「小说创作」。

## 功能

- 主代理直接写作和审核，不启动子代理。
- 保留八项质量检查：设定与边界、人物、章节契约、视角与文风、交付与衔接、重复表达、情节逻辑与伏笔、动作与时间逻辑。
- 修复次数有上限。未解决的硬伤会保留为待修草稿，不会为了通过而降低质量门槛。
- 沿用项目现有的 Bible、人物、时间线和伏笔记录。

## 安装

1. 在本仓库点 **Code → Download ZIP** 并解压，或使用 `git clone` 克隆仓库。
2. 在 DeepSeek Harness 打开 **插件 → 添加插件**，选择解压后的 `dsh-novel-mysolo` 文件夹。如果界面要求路径，填写该文件夹的绝对路径。
3. 新建会话时选择 **小说创作**（`novel-mysolo`）预设。

安装后请保留该文件夹，因为桌面端插件管理器可能会链接到这个目录。修改插件文件后，重启 DeepSeek Harness。

插件没有运行时依赖，不连接原版 `dsh-novel-solo` 包或其更新源。当前以本地源码目录方式安装；`package.json` 中的 `private: true` 用于避免误发布到 npm。

## 自定义

编辑 `template/persona.md` 可调整写作与审核规则。插件面向 DeepSeek Harness `0.2.1-rc.2` 或更新版本，版本要求见 `package.json`。

## 许可证与来源

本定制版本包含基于 Tkingxiao 的 `dsh-novel-solo` 修改的代码。原 MIT 版权和许可保留在 [LICENSE](LICENSE) 中，来源说明见 [NOTICE.md](NOTICE.md)。包身份、运行时依赖和更新路径均已独立。

这是社区插件，不是 DeepSeek Harness 官方产品。
