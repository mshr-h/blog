---
title: "Jupyter Notebook上に現在のノートブックのメモリ使用量を表示する"
slug: "display-memory-usage-on-jupyter-notebook"
subtitle:    ""
description: ""
date:        "2019-03-10"
author:      "Masahiro Hiramori"
image:       ""
tags:        []
categories:  ["Tech" ]
draft:       false
---

Jupyter Notebook上でPythonコードを実行中に、メモリ使用量を確認したいときがある。次のプラグインをインストールすると、Jupyter Notebook上にメモリ使用量を表示できる。

- [yuvipanda/nbresuse](https://github.com/yuvipanda/nbresuse)

インストール方法は次のコマンドを実行する。

```
pip install nbresuse
```

Jupyter Notebookを起動すると、下図赤枠のようにメモリ使用量が表示さる。

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c8e41106-2f0d-4f54-9d84-6f483a8559cc/v08bjzbim52rf21d5vkd.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c8e41106-2f0d-4f54-9d84-6f483a8559cc/v08bjzbim52rf21d5vkd.png)