cmake_format hook for pre-commit
================================

For pre-commit: see https://github.com/pre-commit/pre-commit

For cmake_format: see https://github.com/cheshirekow/cmake_format


### Using cmake_format with pre-commit

Add this to your `.pre-commit-config.yaml`:

    - repo: https://github.com/aharrison24/cmake-format-pre-commit.git
      rev: 'v0.5.5' # Use the sha / tag you want to point at
      hooks:
        - id: cmake-format
          args: [--in-place]


### Repository maintenance
When a new version of cmake_format is released, this repo needs a new commit
with a corresponding tag. This is done with the `bumpversion` app, which is
easily obtained through `pip`:
```bash
pip3 install bumpversion
```

Generate a new commit and tag by calling bumpversion like this:
```bash
bumpversion --new-version 0.5.5 major
```
