# clang-format-precommit

A [pre-commit](https://pre-commit.com) hook to apply
[clang-format](https://clang.llvm.org/docs/ClangFormat.html) using
[wheels](https://github.com/ssciwr/clang-format-wheel).

To use on a repository containing C, C++, or C# files and containing a `.clang-format` style file:

```yml
repos:
- repo: https://github.com/ssciwr/clang-format-hook
  rev: v13.0.0
  hooks:
  - id: clang-format
```

You can override any hook setting if you need to. If you override `args:`, be
sure you include `-i`. If you override types, be sure to use `types_or:`. See
the pre-commit docs for more information.

## Making a new release

To make a new release, update `setup.py`'s pin, as well as this readme, then
make a GitHub release creating a new tag of the form `v<version>`.
