# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__j1mq17a9
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0034065600000000003

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

- **cost**: 0.0034065600000000003
- **output**: ```python
def elevation_angle(location1: "Location", location2: "Location", radians: float=False) -> Optional[float]:
    """ Uphill/downhill angle between two locations. """
    if location1.elevatio...
- **rewrite**: def elevation_angle(location1: "Location", location2: "Location", radians: float=False) -> Optional[float]:
    """ Uphill/downhill angle between two locations. """
    if location1.elevation is None ...
- **strategy**: llm
