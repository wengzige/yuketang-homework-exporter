# yuketang-homework-exporter

<p align="center">
  <img src="assets/release-cover.svg" alt="yuketang-homework-exporter cover" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-2F5D8A?style=flat-square" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/Platform-%E9%9B%A8%E8%AF%BE%E5%A0%82-EA7A2F?style=flat-square" alt="Rain Classroom">
  <img src="https://img.shields.io/badge/Browser-Edge%20%7C%20Chrome-3B7DDD?style=flat-square" alt="Edge and Chrome">
  <img src="https://img.shields.io/badge/Output-Word%20.docx-3FA86B?style=flat-square" alt="Word docx">
  <img src="https://img.shields.io/badge/License-MIT-111827?style=flat-square" alt="MIT License">
</p>

<p align="center">
  <a href="README.zh-CN.md">简体中文</a>
  ·
  <a href="README.en.md">English</a>
</p>

> Export Rain Classroom assignments into a polished Word review pack by reusing your local browser session.
>
> 复用你本机浏览器里已经登录好的雨课堂，把课程作业自动整理成一个可复习、可归档的 Word 文档。

## 中文简介

`yuketang-homework-exporter` 是一个专门面向 **雨课堂** 的作业导出工具。

它会：

- 复用你本机浏览器里已经登录的雨课堂会话
- 自动找到课程里的作业
- 用网页原始效果渲染题目截图，避免加密字体乱码
- 把题目、你的作答、平台判定结果、得分整理进一个 `.docx`

最简单的用法：

```bash
python export_yuketang_homework.py --course-url "把这里替换成你的课程链接" --output-dir output
```

完整中文说明见 [README.zh-CN.md](README.zh-CN.md)。

## English Summary

`yuketang-homework-exporter` is a **Rain Classroom-specific** homework export tool.

It can:

- reuse your already logged-in local browser session
- discover assignment items from a course automatically
- render question screenshots with the original web fonts to avoid garbled text
- assemble questions, your submitted answers, platform verdicts, and scores into one `.docx`

The simplest command:

```bash
python export_yuketang_homework.py --course-url "replace this with your course URL" --output-dir output
```

Full English documentation: [README.en.md](README.en.md).

## Highlights

- Built specifically for **Rain Classroom / 雨课堂**
- No manual cookie or token copying
- Works with `Edge` and `Chrome`
- Solves encrypted font rendering by using browser-rendered screenshots
- Outputs a Word document that is easier to review, archive, or print
- Defaults to a privacy-friendlier workflow: no raw JSON or image dumps unless explicitly requested

## Quick Start

1. Log in to Rain Classroom in your local browser.
2. Copy the course `studentLog` URL.
3. Close the browser if that profile is currently in use.
4. Install dependencies:

```bash
pip install -r requirements.txt
```

5. Run:

```bash
python export_yuketang_homework.py --course-url "your course URL" --output-dir output
```

## Documentation

- 中文文档: [README.zh-CN.md](README.zh-CN.md)
- English docs: [README.en.md](README.en.md)
- GitHub metadata copy: [docs/repo-metadata.md](docs/repo-metadata.md)
- Release template: [docs/release-template.md](docs/release-template.md)

## Privacy Notes

- The script itself does not hardcode your password, cookies, or tokens.
- It reuses the browser profile on your machine, so keep that in mind before recording demos or sharing logs.
- Do not commit your generated `output/`, `.docx`, `raw_json/`, or `images/` files to GitHub.

## Compliance Reminder

Please only export content you are authorized to access, and check:

- Rain Classroom platform terms
- your school or course rules
- whether course materials may be redistributed

## License

[MIT](LICENSE)
