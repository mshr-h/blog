---
title: "2020 08 03 Build Mlir Emitc"
slug: "build-mlir-emitc"
subtitle:    ""
description: ""
date:        "2020-08-03"
author:      "Masahiro Hiramori"
image:       ""
tags:        []
categories:  ["Tech"]
draft:       false
---

```
$ cd ~/workspace
$ git clone https://github.com/iml130/mlir-emitc/
```

```
$ export MLIR_DIR=$(pwd)/llvm-project/build/lib/cmake/mlir
$ export LLVM_EXTERNAL_LIT~$(pwd)/llvm-project/build/bin/llvm-lit
```

```
$ mkdir mlir-emitc/build && cd mlir-emitc/build
$ cmake -G Ninja -DCMAKE_C_COMPILER=clang -DCMAKE_CXX_COMPILER=clang++ .. \
  -DMLIR_DIR=$MLIR_DIR \
  -DLLVM_EXTERNAL_LIT=$LLVM_EXTERNAL_LIT
$ cmake --build . --target check-emitc
```
