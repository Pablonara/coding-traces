# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__be4dx0cj
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0033841300000000004

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

- **cost**: 0.0033841300000000004
- **output**: ```python
def distance_from_line(point: "Location", line_point_1: "Location", line_point_2: "Location") -> Optional[float]:
    """ Distance of point from a line given with two points. """
    assert ...
- **rewrite**: def distance_from_line(point: "Location", line_point_1: "Location", line_point_2: "Location") -> Optional[float]:
    """ Distance of point from a line given with two points. """
    assert point, poi...
- **strategy**: llm
