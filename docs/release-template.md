# Release Template

下面提供一个首发 release 的可复制模板，你可以在 GitHub Release 页面直接用。

## Suggested First Release Title

```text
v0.1.0 - First public release
```

如果你更想保留中文语境，也可以用：

```text
v0.1.0 - 雨课堂作业导出工具首发版
```

## Suggested Release Notes

### Bilingual version

```md
## Overview

First public release of `yuketang-homework-exporter`.

This version focuses on one thing: exporting Rain Classroom assignments into a Word review document by reusing a locally logged-in browser session.

## What’s included

- support for Rain Classroom course assignment export
- browser-session reuse through Edge or Chrome
- browser-rendered question screenshots to avoid encrypted-font garbling
- Word `.docx` output with:
  - question screenshots
  - your submitted answers
  - platform verdicts
  - scores
- optional raw JSON export
- optional screenshot export
- bilingual documentation

## Notes

- Please only export content you are authorized to access.
- Do not commit generated `output/`, `.docx`, `raw_json/`, or `images/` files to your repository.
- If your browser profile is currently open, close the browser first before running the script.

## 中文说明

这是 `yuketang-homework-exporter` 的首个公开版本。

这个版本主要解决一个问题：复用本机已登录浏览器会话，把雨课堂课程作业整理成 Word 复习文档。

包含内容：

- 支持雨课堂课程作业导出
- 支持 Edge / Chrome 登录态复用
- 通过浏览器渲染题目截图，避免加密字体乱码
- 输出 Word 文档，包含：
  - 题目截图
  - 我的作答
  - 平台判定结果
  - 得分
- 可选保存原始 JSON
- 可选保存题目截图
- 提供中英双语文档
```

### Short version

```md
First public release of `yuketang-homework-exporter`.

Highlights:

- Rain Classroom assignment export
- Edge / Chrome session reuse
- screenshot-based question rendering for encrypted fonts
- Word `.docx` output with answers, verdicts, and scores
- bilingual documentation
```

## Suggested Release Assets

如果你准备给 release 配图或附件，可以考虑：

- `assets/release-cover.png`
- 打包后的源码压缩包
- 如果你以后做了 GUI 版，也可以把可执行文件挂在这里
