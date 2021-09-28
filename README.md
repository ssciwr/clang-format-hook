# clang-format-precommit

A [pre-commit](https://pre-commit.com) hook to apply
[clang-format](https://clang.llvm.org/docs/ClangFormat.html) using
[wheels](https://github.com/ssciwr/clang-format-wheel).

To use on a repository containing C, C++, or C# files and containing a `.clang-format` style file:

```yml
repos:
- repo: https://github.com/pre-commit/pre-commit-hooks
  rev: v11.0.1
  hooks:
  - pre-commit
```

You can override any hook setting if you need to. If you override `args:`, be
sure you include `-i`. If you override types, be sure to use `types_or:`. See
the pre-commit docs for more information.
