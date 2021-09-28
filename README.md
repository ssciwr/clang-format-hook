# clang-format-precommit

A [pre-commit](https://pre-commit.com) hook to apply
[clang-format](https://clang.llvm.org/docs/ClangFormat.html) using
[wheels](https://github.com/ssciwr/clang-format-wheel).

To use on a repository containing C, C++, or C# files and containing a `.clang-format` style file:

```yml
repos:
- repo: https://github.com/ssciwr/clang-format-precommit
  rev: v12.0.1
  hooks:
  - id: clang-format
```

You can override any hook setting if you need to. If you override `args:`, be
sure you include `-i`. If you override types, be sure to use `types_or:`. See
the pre-commit docs for more information.
