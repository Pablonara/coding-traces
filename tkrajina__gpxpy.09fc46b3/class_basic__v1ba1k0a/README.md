# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__v1ba1k0a
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0038238600000000005

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

- **cost**: 0.0038238600000000005
- **output**: ```python
def length_3d(locations: List["Location"]=[]) -> float:
    """ 3-dimensional length (meters) of locations (it uses latitude, longitude, and elevation). """
    return length(locations, Fals...
- **rewrite**: def length_3d(locations: List["Location"]=[]) -> float:
    """ 3-dimensional length (meters) of locations (it uses latitude, longitude, and elevation). """
    return length(locations, False)
- **strategy**: llm
