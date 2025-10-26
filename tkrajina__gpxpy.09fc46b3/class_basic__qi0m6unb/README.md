# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__qi0m6unb
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.007766360000000001

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

- **cost**: 0.007766360000000001
- **output**: ```python
def get_line_equation_coefficients(location1: "Location", location2: "Location") -> Iterable[float]:
    """
    Get line equation coefficients for:
        latitude * a + longitude * b + c ...
- **rewrite**: def get_line_equation_coefficients(location1: "Location", location2: "Location") -> Iterable[float]:
    """
    Get line equation coefficients for:
        latitude * a + longitude * b + c = 0

    T...
- **strategy**: llm
