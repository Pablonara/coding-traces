# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__tyx8onx6
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.005401700000000001

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

- **cost**: 0.005401700000000001
- **output**: ```python
def calculate_max_speed(speeds_and_distances: List[Tuple[float, float]], extreemes_percentile: float, ignore_nonstandard_distances: bool) -> Optional[float]:
    """
    Compute average dist...
- **rewrite**: def calculate_max_speed(speeds_and_distances: List[Tuple[float, float]], extreemes_percentile: float, ignore_nonstandard_distances: bool) -> Optional[float]:
    """
    Compute average distance and s...
- **strategy**: llm
