cmake_format hook for pre-commit
================================

For pre-commit: see https://github.com/pre-commit/pre-commit

For cmake_format: see https://github.com/cheshirekow/cmake_format


### Using cmake_format with pre-commit

Add this to your `.pre-commit-config.yaml`:

    - repo: https://github.com/aharrison24/cmake-format-pre-commit.git
      rev: 'v0.5.1' # Use the sha / tag you want to point at
      hooks:
        - id: cmake-format
          args: [--in-place]
