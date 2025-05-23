# SJTUThesis 示例模板

[![Build Status](https://github.com/sjtug/SJTUThesis/actions/workflows/build.yml/badge.svg)](https://github.com/sjtug/SJTUThesis/actions)
[![SJTUTeX](https://img.shields.io/github/v/release/sjtug/SJTUTeX?label=SJTUTeX)](https://github.com/sjtug/SJTUTeX)
[![Join Discussions](https://img.shields.io/github/discussions/sjtug/SJTUThesis)](https://github.com/sjtug/SJTUThesis/discussions)

## 欢迎使用上海交通大学论文模板

本示例模板是应用上海交通大学学位论文 LaTeX 文档类 SJTUThesis 的一个完整实现。演示了排版中常用的例子，包括公式、表格、算法、参考文献等。
用户可以参考或者直接基于此示例文档撰写论文。

SJTUThesis 支持 XeTeX 与 LuaTeX 引擎，字符编码仅支持 UTF-8。

## 安装 TeX 发行版

由于 SJTUThesis 依赖的文档类集 SJTUTeX 已经被 [CTAN](https://www.ctan.org/pkg/sjtutex) 收录，你需要首先按照 [安装指南](https://github.com/sjtug/SJTUThesis/wiki/TeX-%E5%8F%91%E8%A1%8C%E7%89%88%E5%8F%8A%E5%85%B6%E5%AE%89%E8%A3%85) 安装**最新版本的 TeX 发行版**，并经常[对宏包进行更新](https://github.com/sjtug/SJTUThesis/wiki/TeX-%E5%8F%91%E8%A1%8C%E7%89%88%E5%8F%8A%E5%85%B6%E5%AE%89%E8%A3%85#%E5%AE%89%E8%A3%85%E6%88%96%E6%9B%B4%E6%96%B0%E5%AE%8F%E5%8C%85)以使用最新版本的 SJTUTeX。

## 获取模板

### 下载模版

你可以直接 `clone` 或者下载 [master.zip](https://github.com/sjtug/SJTUThesis/archive/refs/heads/master.zip)。

```bash
git clone https://github.com/sjtug/SJTUThesis.git
# ...or with SJTUG mirror
git clone https://mirror.sjtu.edu.cn/git/SJTUThesis.git/
```

模版更新频繁，且只维护最新版。如有问题，可以先尝试升级模版，而后根据“反馈问题”一栏进行反馈。

### 在线 LaTeX 编辑器

[![TeXPage](https://img.shields.io/badge/SJTUThesis-TeXPage-495A80.svg)](https://www.texpage.com/template/542af6f9-f66f-4068-8732-f20fe7bd08ef)

[![Overleaf](https://img.shields.io/badge/SJTUThesis-Overleaf-098842.svg)](https://www.overleaf.com/latex/templates/sjtuthesis-latex-thesis-template-for-shanghai-jiao-tong-university/mkdwbyjbtfgg)

点击上方图标即可直接使用。

如果你需要在其他支持最新 TeX 发行版的在线 LaTeX 编辑器上使用（比如 [SJTU LaTeX 文档助手](https://latex.sjtu.edu.cn)），你可以下载 [最新版压缩包](https://github.com/sjtug/SJTUThesis/archive/refs/heads/master.zip)，然后上传至相应平台。请注意，一般在线编辑器新建项目默认使用 pdfLaTeX 编译器，你需要设置使用 XeLaTeX 编译器；并使用最新的 TeX 发行版本。

## 模板使用

如果你不熟悉 LaTeX 的编译流程，请参考以下说明编译文档。

### 使用编辑器

#### VS Code

安装 “LaTeX Workshop” 扩展，选择预设配方 `Recipe: latexmk (xelatex)` 编译即可；也可以在设置中将 `latex-workshop.latex.recipe.default` 改为 `latexmk (xelatex)` 将其设置为默认选项。

#### TeXstudio

模板内置 TeXstudio 魔术注释，可开箱即用。

### 使用脚本

#### Linux 与 macOS

推荐使用模版提供的 `Makefile` 进行编译，具体来说我们提供了如下几条可用的命令：

```bash
make all                      # 编译生成 main.pdf
make clean                    # 删除编译所产生的中间文件
make cleanall                 # 删除 main.pdf 和所有中间文件
make wordcount                # 论文字数统计
```

#### Windows

对于 Windows 用户，我们也提供了编译脚本 `Compile.bat`。可以双击直接编译，也可以在命令提示符窗口中使用脚本提供的额外功能：

```bash
.\Compile.bat thesis          # 编译生成 main.pdf
.\Compile.bat clean           # 删除编译所产生的中间文件
.\Compile.bat cleanall        # 删除 main.pdf 和所有中间文件
.\Compile.bat wordcount       # 论文字数统计
```

更多关于模板的实现细节以及使用信息，请查看使用文档 [`sjtutex.pdf`](https://mirrors.ctan.org/macros/latex/contrib/sjtutex/sjtutex.pdf)。

## 反馈与贡献

本模版是由诸多感兴趣的同学一起维护的开源项目，我们非常欢迎问题反馈和新的贡献者！

### 反馈问题

如果在使用上有任何问题，建议先查阅项目的 [Wiki 文档](https://github.com/sjtug/SJTUThesis/wiki)，并使用左上角的搜索功能进行搜索。
如果以上方法不能解决你的问题，建议通过以下方式进行反馈（按推荐顺序排序）：

* 如遇不会使用、编译错误等问题，请至 [在 GitHub 项目讨论区提问](https://github.com/sjtug/SJTUThesis/discussions) (推荐)
* 如遇模版 BUG，或有新的需求，请至 [在 GitHub 项目中提 issue](https://github.com/sjtug/SJTUThesis/issues)
* 你也可以加入 SJTUG 的 QQ 群和 Telegram 群即时讨论。
    * QQ 群群号 715273806。
    * Telegram 群。首先，关注 [SJTUG 镜像站的通知频道](https://t.me/sjtug_mirrors_news)。而后，加入频道关联的群组。

### 成为贡献者

这个仓库是面向用户的**示例模版**，如果你有很好的排版示例，可以提交到此仓库与大家分享。如果你想要为 SJTUThesis 文档类贡献代码，可移步 [SJTUTeX](https://github.com/sjtug/SJTUTeX)。

在贡献之前，你可以从[这些问题](https://github.com/sjtug/SJTUThesis/issues?q=is%3Aissue+is%3Aopen+label%3Agood-first-issue)开始熟悉贡献代码的流程。除了提交 Pull Request 之外，还有以下方式可以进行贡献：

* 帮助我们解答同学们的[问题](https://github.com/sjtug/SJTUThesis/discussions)，这些问题你也可能遇到过并且知道如何解决；
* 与我们一起维护项目的 [Wiki 文档](https://github.com/sjtug/SJTUThesis/wiki)，Wiki 任何人都可以直接编辑；
* 向周围同学安利 SJTUThesis，让更多的同学使用我们维护的模板；
* 在我们的讨论组中分享你的使用体验，以及吐槽。如果你也想成为项目的长期维护者，也可以通过讨论组告诉我们。:-)


## 致谢

* 感谢 [CTeX-kit](https://github.com/CTeX-org/ctex-kit) 提供了 LaTeX 的中文支持；
* 感谢那位最先制作出博士学位论文 LaTeX 模板的物理系同学；
* 感谢 William Wang 同学对模板移植做出的贡献；
* 感谢 [@weijianwen](https://github.com/weijianwen) 学长开创性的工作；
* 感谢 [@sjtug](https://github.com/sjtug) 对 0.10 及之后版本的开发和维护工作；
* 感谢所有为模板贡献过代码的[同学们](https://github.com/sjtug/SJTUThesis/graphs/contributors)，以及所有测试和使用模板的各位同学。

## 软件许可证

上海交通大学校徽校名图片（`sjtu-vi-logo-*.pdf` 等）的版权归上海交通大学所有。

`sjtutex` 文档类集（`sjtuthesis.cls` 等）使用 [The LaTeX Project Public License 1.3c](https://www.latex-project.org/lppl.txt) 授权。

其他部分使用 [Apache License 2.0](LICENSE) 授权。
