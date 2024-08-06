---
title: 基于Antora的文档框架说明
date: 2024-03-20
categories: 关于产品文档
top: 200
---

# 文档架构说明

![avatar](/images/antora.png)

Antora是一个开源的文档生成工具，专注于构建技术文档。它使用 AsciiDoc 作为其主要的标记语言，并结合 Git 作为版本控制系统，提供了强大的文档管理和协作功能。

具体来说，这套系统的组成部分如下：

1. **Antora**：
   - Antora 是一个基于 Node.js 的静态站点生成器，专门用于构建技术文档。它允许你从多个源（如 Git 仓库）收集文档内容，并根据配置生成一个完整的静态网站。
   - Antora 支持模块化的文档结构，可以将文档分解为多个独立的模块（或组件），每个模块都有自己的版本控制和发布流程。
   - Antora 使用 AsciiDoc 作为默认的标记语言，AsciiDoc 是一种功能强大的文档标记语言，支持结构化内容、内部链接、图表和代码示例等丰富的功能。

2. **AsciiDoctor**：
   - AsciiDoctor 是一个开源的文档处理器，用于将 AsciiDoc 标记转换为各种输出格式，包括 HTML、PDF 和 ePub 等。它是 Antora 使用的默认渲染引擎，负责将 AsciiDoc 标记转换为静态网页。

3. **Git**：
   - Git 是一个分布式版本控制系统，用于管理文档的源代码和版本历史。在 Antora 中，Git 被用来存储和跟踪文档的所有更改，每个文档模块都可以作为一个独立的 Git 仓库进行管理。
   - Git 提供了强大的分支和合并功能，使得团队可以并行开发和维护多个文档版本，而不会出现冲突或丢失历史记录。

# 相关链接

- https://antora.org/
- https://antora.zulipchat.com/
- https://docs.asciidoctor.org/asciidoctor/latest/