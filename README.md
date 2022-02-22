# clang-format pre-commit hook

This repository contains a [pre-commit](https://pre-commit.com) hook to apply
[clang-format](https://clang.llvm.org/docs/ClangFormat.html) using
[wheels](https://github.com/ssciwr/clang-format-wheel).

In contrast to [https://github.com/pre-commit/mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format),
this repository provides backports of older versions of clang-format.
Use this if you need to stick to a specific major/minor version of clang-format.
