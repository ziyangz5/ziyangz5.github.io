---
title: 'TorchLib + CMake + Windows = 0xc0000135'
date: 2199-01-01
permalink: /posts/2023/07/blog-post-1/
tags:
  - Log
  - CUDA
  - TorchLib
---

Passed compiling. Unable to run with exit code 0xc0000135. Turns out that the cmake configuration is slightly different on windows.

Instead of adding "C:\\PATH\\TO\\libtorch" to the CMAKE_PREFIX_PATH, you need to add "C:\\PATH\\TO\\libtorch\\lib".

Added. Problem solved.
