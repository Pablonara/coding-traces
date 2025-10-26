# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__g6liwfu2
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0023072

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

- **cost**: 0.0023072
- **output**: ```python
def __str__(self) -> str:
    if hasattr(self, 'distance'):
        return f'LocationDelta(distance={self.distance}, ' \
               f'angle={self.angle_from_north})'
    return f'Locatio...
- **rewrite**: def __str__(self) -> str:
    if hasattr(self, 'distance'):
        return f'LocationDelta(distance={self.distance}, ' \
               f'angle={self.angle_from_north})'
    return f'LocationDelta(lat...
- **strategy**: llm
