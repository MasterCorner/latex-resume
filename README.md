# 📄 LaTeX 双语简历源码 (Bilingual Resume Source)

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Compiler](https://img.shields.io/badge/compiler-XeLaTeX-red)
![License](https://img.shields.io/badge/license-LPPL-lightgrey)

这是 **王睿敏 (Ruimin Wang)** 的个人简历源码仓库。
本项目基于 LaTeX 模板定制，支持在同一个项目结构中编译**中文**和**英文**两个版本的简历。

> **🔗 在线预览 / Live Preview**: [resume.chiikawa.asia](https://resume.chiikawa.asia)

---

## ✨ 项目亮点 (Key Features)

- **双语架构**：单一项目管理中文 (`main_cn.tex`) 和英文 (`main_en.tex`) 两个版本，共用样式和资源。
- **深度定制**: 基于 `.cls` 文件进行了定制，修复了图标对齐问题，并增加了网页预览支持。
- **模块化设计**: 教育、工作经历等内容独立分块，便于维护。
- **工程化规范**: 标准的 Git 管理与文件结构。

## 📂 目录结构 (Structure)

```text
.
├── fonts/                   # 编译所需的中文字体文件 (Adobe)
├── images/                  # 头像及其他图片资源
├── my-custom-cv.cls         # [核心] 定制后的样式文件
├── main_cn.tex              # 中文简历入口
├── main_en.tex              # 英文简历入口
├── section_education_cn.tex # 教育经历 (中文)
├── section_education_en.tex # Educational Background (English)
├── ...                      # 其他章节文件
└── README.md
```

## 🚀 如何编译 (How to Build)
本项目使用 XeLaTeX 引擎。你可以在本地 (TeX Live / MacTeX) 或 Overleaf 上编译。

前置要求 (Prerequisites)
请确保项目的 `fonts/` 目录下包含必要的中文字体文件（如 Adobe Song/Heiti 等），或者你的操作系统已安装这些字体。

编译命令 (Build Commands)
生成中文版:
```bash
xelatex main_cn.tex
```
生成英文版:
```bash
xelatex main_en.tex
```
注意：通常需要连续编译两次，以确保页码或目录链接跳转正确。

## 👏 致谢 (Credits)
本项目基于开源社区成果修改，特别感谢：
- 模板基础: Awesome Latex CV by Junhao Hua & Christophe Roger.
- 字体支持: 中文字体支持方案 (`zh_cn-adobefonts_external.sty`) 及字体库引用自 billryan/resume 项目。

## ⚖️ 开源协议 (License)
代码部分: 模板代码 (`.cls` 文件及结构) 遵循 LaTeX Project Public License (LPPL) 1.3c 协议。详情请见 LICENSE 文件。
内容部分: 简历的具体内容（文字、个人信息、图片）版权归 王睿敏 所有。 (Content Copyright © 2025 Ruimin Wang. All rights reserved.)
