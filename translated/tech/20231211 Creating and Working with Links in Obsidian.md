[#]: subject: "Creating and Working with Links in Obsidian"
[#]: via: "https://itsfoss.com/obsidian-create-links/"
[#]: author: "Sreenath https://itsfoss.com/author/sreenath/"
[#]: collector: "lujun9972/lctt-scripts-1700446145"
[#]: translator: "geekpi"
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

在 Obsidian 中创建和使用链接
======

Obsidian 的最卖点之一是其强大的文档链接和可视化。Obsidian 提供了多种链接文档和图像的方法。我们将逐一介绍。

你将在 Obsidian 中看到三种内部链接方法：

   * 拖放方式（简单但有限）
   * 使用 Markdown 链接
   * 使用维基链接（广泛且强大）



我还将分享一些有关使用图表和反向链接的技巧。让我们来看看它。

✋

****非自由和开源软件警告！**** Obsidian 不是开源软件，我们知道这一事实。然而，它是一种在编码人员（包括开源开发人员）中非常流行的工具。这就是我们介绍它的原因。

### 方法 1：通过拖放链接

是的，这是最简单的链接。转到要在其中创建链接的文档。现在，在左侧边栏上，展开该特定文件夹，其中包含目标注释。

要创建链接，只需将此目标文件拖放到你希望链接显示的位置即可。

![通过拖放添加链接][1]

你可以稍后更改链接文本。

### 方法 2：使用 Markdown 链接

由于 Obsidian 使用 Markdown 作为其核心，因此可以通过输入传统的 Markdown 命令进行链接。

比方说，你必须在 “Markdown Advanced” 页面中创建一个指向 “Markdown Checklist” 页面的链接。首先，你需要记下要链接到的文件的位置。

然后，只需添加这一行：

````

     [链接文本]（文件的相对路径）

````

或者，如果你有要链接的文件，并且想要提供系统中的绝对路径，请使用：

````

     [链接文本](file://绝对路径)

````

![使用绝对路径链接][2]

🚧

如果你[使用 Markdown 链接][3]，请确保文件和文件夹的名称中没有空格，因为这在某些情况下可能会引起一些麻烦。

### 方法 3：使用紧凑型 Wikilink 链接页面

Obsidian 支持使用 [Wikilinks][4] 链接页面的直观方式。它们是紧凑的链接并且是交互式链接。默认情况下，此功能处于打开状态。

如果你想知道，是的，它与维基百科有关。他们用它来内部链接他们的维基页面。

#### 添加内部注释的链接

要创建链接，只需输入 `[[`。这将启动一个交互式对话框，你可以在其中搜索要链接的文档。

![添加交互式维基链接][5]

💡

你可以使用 [[link|要显示的文本]]使自定义文本显示在 Wikilink 上。例如 [[notes/hello.md|这是 Hello 文件的链接]]

#### 添加图像文件

此外，你可以使用此链接方法添加其他文件，例如图像，但在使用 `[[` 搜索之前需要添加 `!` 符号。请看下图以了解其实际效果。

![使用 Wikilink 添加图像][6]

#### 添加内部标题链接

有一种方法可以在同一页面的各个标题之间创建内部链接。为此，首先输入 `[[`，然后使用 Markdown 标题语法和要链接的特定标题的名称。

例如，如果你打算链接到文档中的第六个标题（2 级标题），请使用：

```

    [[##Paragraph Six

```

这将显示在交互式选择中。

![链接到标题][7]

💡

你可以将鼠标悬停在链接上时按 CTRL 键来进行预览。

#### 添加指向文本块的链接

Obsidian 允许你创建指向文档中特定文本块的链接。为此，首先，转到要添加链接的块的最末尾。

现在，使用 `^` 符号向该块添加唯一标识符。

![向块添加唯一标识符][8]

现在，你可以通过输入 `[[^` 来添加到此部分的链接。这将自动提示你可用的块。选择一项并按回车键。

![添加链接到块][9]

#### Wikilink 问题

有时，如果你想要纯 Markdown 文档，并且专注于多个 Markdown 编辑器之间的互操作性，那么 Wikilinks 功能可能会产生问题。

由于这些在 Obsidian 内部工作，因此链接在其他编辑器上显示为损坏。在这种情况下，你可以关闭 Wikilink。一切都完美无缺，只是链接现在将以 Markdown 格式显示。

为此，首先选择左下角的设置按钮。

![点击设置][10]

现在，从“文件和链接”选项卡关闭 Wikilink 功能。

![关闭 Wikilinks 功能][11]

#### 组织附件文件的提示

对于那些在 Obsidian 中附加许多文件的人，建议在每本书下为这些附件创建一个单独的文件夹。

现在，打开**设置>文件和链接**。在这里，首先，你需要确保链接路径是相对于文件位置的。然后，将新附件的默认位置设置为“当前文件夹下的子文件夹”。现在，在下一个字段中指定“附件”，即“子文件夹名称”。

![设置附件文件夹位置][12]

就是这样。从现在开始，当你通过复制和粘贴放置任何附件时，它们将自动放置在该笔记文件夹内的“附件”文件夹中。新链接将在任何 Markdown 编辑器之间完美地互操作，因为路径现在是相对于文件位置的。

📋

即使此 Wikilink 功能已关闭，你仍然可以使用 [[ 键以交互方式搜索和添加链接。变化是，现在链接不再是紧凑的，而是长 Markdown 链接。

此外，你还可以打开“自动更新内部链接”按钮，以确保在重命名文件时自动更新链接。

###

### 使用图表和反向链接

创建完链接后，就可以通过链接查看笔记之间的其他笔记之间的关系。单击侧面的图表视图按钮即可进入图表预览。

![Obsidian 中的图表视图][13]

正如你所看到的，你将在一个整洁的图表上获得该注释的链接。如果你按空白选项卡上的图表视图，你将获得所有笔记及其关系。

![Notes Vault 示例的一些链接示例][14]

此外，每个笔记都有一“传出链接”和“传入链接”选项卡，你可以在其中跟踪相关链接。

![传出和传入链接][15]

### 结论

正如你所看到的，虽然在 Obsidian 中创建指向其他页面的内部链接很简单，但通过 Wikilinks，你可以创建更加个性化和定制的知识库。

对于那些不喜欢 Obsidian 闭源性质的人来说，[Logseq][16] 是一个不错的选择。

![][17]

--------------------------------------------------------------------------------

via: https://itsfoss.com/obsidian-create-links/

作者：[Sreenath][a]
选题：[lujun9972][b]
译者：[geekpi](https://github.com/geekpi)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://itsfoss.com/author/sreenath/
[b]: https://github.com/lujun9972
[1]: https://itsfoss.com/content/images/2023/12/link-by-drag-and-drop.gif
[2]: https://itsfoss.com/content/images/2023/12/linking-using-absolute-path.png
[3]: https://itsfoss.com/markdown-links/
[4]: https://en.wikipedia.org/wiki/Help:Link
[5]: https://itsfoss.com/content/images/2023/12/add-interactive-wikilinks.gif
[6]: https://itsfoss.com/content/images/2023/12/add-image-using-wikilinks.gif
[7]: https://itsfoss.com/content/images/2023/12/Link-to-heading-1.gif
[8]: https://itsfoss.com/content/images/2023/12/Add-unique-identifier-to-a-block.png
[9]: https://itsfoss.com/content/images/2023/12/your-block-link.gif
[10]: https://itsfoss.com/content/images/2023/12/click-on-settings-button-in-obsidian.png
[11]: https://itsfoss.com/content/images/2023/12/turn-off-the-wikilink-feature.png
[12]: https://itsfoss.com/content/images/2023/12/set-attachment-folder-location-and-other-settings-1.png
[13]: https://itsfoss.com/content/images/2023/12/graph-view-in-obsidian.png
[14]: https://itsfoss.com/content/images/2023/12/part-of-a-graph-view.png
[15]: https://itsfoss.com/content/images/2023/12/Links-out-and-in.png
[16]: https://itsfoss.com/logseq/
[17]: https://itsfoss.com/content/images/size/w256h256/2022/12/android-chrome-192x192.png
