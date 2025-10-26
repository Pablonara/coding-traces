# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__l99rle2j
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.006876760000000001

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

- **cost**: 0.006876760000000001
- **output**: ```python
def __init__(self, distance: Optional[float]=None, angle: Optional[float]=None,
             latitude_diff: Optional[float]=None,longitude_diff: Optional[float]=None) -> None:
    """
    Ve...
- **rewrite**: def __init__(self, distance: Optional[float]=None, angle: Optional[float]=None,
             latitude_diff: Optional[float]=None,longitude_diff: Optional[float]=None) -> None:
    """
    Version 1:
 ...
- **strategy**: llm
