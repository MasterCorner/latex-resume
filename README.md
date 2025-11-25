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
