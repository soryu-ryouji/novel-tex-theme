<div align=center>
    <img src="./.assets/novel-tex-logo.png">
</div>

# Novel Tex

> Novel Tex 是基于 [typora-latex-theme](https://github.com/Keldos-Li/typora-latex-theme) 的修改版本，沿用 GPL 3.0 许可证。

主要修改：

1. 提取出了 typora-latex-theme 的标题自动编号特性
2. 修改了 typora-latex-theme 的页面大小与字体大小，优化了笔记本设备的使用体验
3. 将 mermaid 的默认主题修改为灰色，使其与主题风格更加统一
4. 增加了代码块线框，使代码块在文档中更加显眼
5. 更改了默认字体

> 如果不需要标题自动编号特性，可在 `novel-tex/basic/include.css` 中注释掉 `@import "./outline.css";`

NovelTex 使用思源宋体作为文档中文字体、Times New Roman 作为文档英文字体、微软雅黑作为 UI 字体、Consolas 作为代码字体。

<!-- 思源黑体：https://github.com/adobe-fonts/source-han-sans/releases/download/2.004R/SourceHanSansSC.zip -->

思源宋体：https://github.com/adobe-fonts/source-han-serif/releases/download/2.002R/09_SourceHanSerifSC.zip

如果不习惯主题的默认字体，或者有特殊的字体需求，可以在 `novel-tex/basic/font.css` 文件中更改主题的字体。

## 主题版本介绍

各个主题文件之间没有相互依赖的关系，可以只复制自己需要的主题文件使用，但 `novel-tex` 文件夹需要完整复制，里面包含了主题文件所需要的基础配置。

### 主题颜色

| Name | Description  |
| ---- | ------------ |
| FD   | Full Dark    |
| ND   | Normal Dark  |
| FL   | Full Light   |
| NL   | Normal Lignt |


## 开发指南

所有基础性的配置全部放入`novel-tex/basic/`中，所有与明暗配置相关的内容放入`novel-tex/dark/`与`novel-tex/light/`中，放在根目录的主题文件只用于修改颜色变量。

```shell
theme/
├─novel-tex/
│   ├─basic/
│   ├─dark/
│   └─light/
├─novel-tex-f-d.css
├─novel-tex-f-l.css
├─novel-tex-n-d.css
└─novel-tex-n-l.css
```

**`novel-tex/basic/` 文件介绍**

- `basic.css`: 放置一些无法被归类的基础配置
- `code.css`: 代码的基础配置，其他的配置在 `novel-tex/dark/` 和 `novel-tex/light/` 中
- `font.css`: 文档字体的配置
- `footnote.css`: 文档脚注的配置
- `include.css`: 所有基础配置的引用
- `list.css`: 文档有序列表和无序列表的配置
- `math.css`: 数学公式的配置
- `mermaid.css`: mermaid 图表配置
- `outline.css`: 文档标题自动编号的配置
- `quote.css`: 文档引言的配置
- `table.css`: 文档表格的配置
- `toc.css`: 文档 `Table of Content` 的配置
- `ui.css`: Typora 的 UI 配置

## Screenshots

> 通过身边使用该主题的朋友反馈，主题样式会不定期更新
>
> 文档中的界面预览图与实际安装后的界面不保证百分百相同（有空时会上传新的预览图）


**Full Light**

![fd](./.assets/novel-tex-f-l.png)

![fd](./.assets/novel-tex-f-l-code.png)

**Normal Light**

![fd](./.assets/novel-tex-n-l.png)

![fd](./.assets/novel-tex-n-l-code.png)

**Full Dark**

![fd](./.assets/novel-tex-f-d.png)

![fd](./.assets/novel-tex-f-d-code.png)

**Normal Dark**

![fd](./.assets/novel-tex-n-d.png)

![fd](./.assets/novel-tex-n-d-code.png)