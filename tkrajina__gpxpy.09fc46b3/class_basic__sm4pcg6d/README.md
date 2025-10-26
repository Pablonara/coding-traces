# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__sm4pcg6d
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.004821880000000001

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

- **cost**: 0.004821880000000001
- **output**: ```python
def move_by_angle_and_distance(self, location: Location) -> Tuple[float, float]:
    coef = mod_math.cos(mod_math.radians(location.latitude))
    vertical_distance_diff = mod_math.sin(mod_ma...
- **rewrite**: def move_by_angle_and_distance(self, location: Location) -> Tuple[float, float]:
    coef = mod_math.cos(mod_math.radians(location.latitude))
    vertical_distance_diff = mod_math.sin(mod_math.radians...
- **strategy**: llm
