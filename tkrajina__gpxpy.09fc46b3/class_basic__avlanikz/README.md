# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__avlanikz
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.005444910000000001

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

- **cost**: 0.005444910000000001
- **output**: ```python
def simplify_polyline(points: List["Location"], max_distance: Optional[float]) -> List["Location"]:
    """Does Ramer-Douglas-Peucker algorithm for simplification of polyline """

    _max_d...
- **rewrite**: def simplify_polyline(points: List["Location"], max_distance: Optional[float]) -> List["Location"]:
    """Does Ramer-Douglas-Peucker algorithm for simplification of polyline """

    _max_distance = ...
- **strategy**: llm
