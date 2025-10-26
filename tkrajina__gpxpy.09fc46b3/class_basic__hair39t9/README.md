# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__hair39t9
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0031641200000000003

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

- **cost**: 0.0031641200000000003
- **output**: ```python
def length_2d(locations: List["Location"]=[]) -> float:
    """ 2-dimensional length (meters) of locations (only latitude and longitude, no elevation). """
    if len(locations) > 1:
       ...
- **rewrite**: def length_2d(locations: List["Location"]=[]) -> float:
    """ 2-dimensional length (meters) of locations (only latitude and longitude, no elevation). """
    if len(locations) > 1:
        return le...
- **strategy**: llm
