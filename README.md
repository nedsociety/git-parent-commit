# git-parent-commit

Finds the latest commit in a parent repository that is compatible with a specific version of a submodule repository.

## Installation

1. Install prerequisites.
2. Download and install the script using the following commands:

```bash
wget https://github.com/nedsociety/git-parent-commit/raw/refs/heads/main/git-parent-commit
sudo install -m 755 git-parent-commit /usr/local/bin/git-parent-commit
```

## Requirements

- Python 3.8 or higher
- [uv](https://github.com/astral-sh/uv)
- Git

## Usage Example

```bash
# Show help
git parent-commit

# Find the latest parent commit that points to a submodule commit
git parent-commit -s <submodule-path> -c <commit-id>

# Find the latest parent commit that points to a compatible submodule commit with respect to some path
git parent-commit -s <submodule-path> -c <commit-id> -p <path1> <path2> <...>
```
