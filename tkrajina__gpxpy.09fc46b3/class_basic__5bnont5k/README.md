# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__5bnont5k
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.00447319

## Bug Description

I've introduced several subtle bugs:

1. **Changed smoothing coefficients**: Modified the smoothing weights from (0.3, 0.4, 0.3) to (0.4, 0.2, 0.4), which changes the smoothing behavior and can produce different elevation profiles.

2. **Removed None check in filter function**: The inner `__filter` function no longer checks if `current_ele` is None, but since we filtered out None values earlier, this doesn't cause immediate errors - just makes the code less robust.

3. **Reversed elevation difference calculation**: Changed `d = cur - prev` to `d = prev - cur`, which reverses the uphill/downhill calculation. Now uphill is calculated when going downhill and vice versa.

4. **Removed None check in loop**: The loop no longer checks if `prev` and `cur` are None, but again, since we filtered out None values earlier, this doesn't cause errors but makes the logic less explicit.

These changes will cause the function to return incorrect uphill and downhill values while maintaining the same interface and not causing any syntax errors.

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

- **cost**: 0.00447319
- **output**: ```python
def calculate_uphill_downhill(elevations: List[Optional[float]]) -> Tuple[float, float]:
    """
    Compute the total uphill and downhill elevation for a list of elevations.
    Note that t...
- **rewrite**: def calculate_uphill_downhill(elevations: List[Optional[float]]) -> Tuple[float, float]:
    """
    Compute the total uphill and downhill elevation for a list of elevations.
    Note that the result ...
- **strategy**: llm
