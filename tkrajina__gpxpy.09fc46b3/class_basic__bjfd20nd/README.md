# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__bjfd20nd
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.004199950000000001

## Bug Description



## Structure

- **repo/**: The repository with the bug applied
- **bug.patch**: The patch file that was applied to create the bug
- **metadata.json**: Complete metadata about the bug
- **summary.json**: Summary information and file paths
- **README.md**: This file

## Usage

### Inspect the bug
```bash
cd repo
git diff HEAD
```

### Revert the bug
```bash
cd repo
git apply -R ../bug.patch
```

### Run tests with the bug
```bash
cd repo
# Run your test suite here
```

### Apply to another clean repository
```bash
git apply ../bug.patch
```

## Metadata

- **cost**: 0.004199950000000001
- **output**: ```python
def __init__(self, min_latitude: Optional[float] = None, max_latitude: Optional[float] = None,
             min_longitude: Optional[float] = None, max_longitude: Optional[float] = None) -> N...
- **rewrite**: def __init__(self, min_latitude: Optional[float] = None, max_latitude: Optional[float] = None,
             min_longitude: Optional[float] = None, max_longitude: Optional[float] = None) -> None:
    s...
- **strategy**: llm
