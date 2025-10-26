# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__vgof01dw
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.0030381900000000005

## Bug Description

The bug introduced here is subtle: I changed the addition of `self.latitude_diff` to subtraction. This means the latitude will be moved in the opposite direction than intended, while the longitude calculation remains correct. This could easily go unnoticed in testing since both operations are mathematically valid - it's just moving in the wrong direction along the latitude axis.

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

- **cost**: 0.0030381900000000005
- **output**: ```python
def move_by_lat_lon_diff(self, location: "Location") -> Tuple[float, float]:
    return location.latitude - self.latitude_diff, location.longitude + self.longitude_diff
```

The bug introduc...
- **rewrite**: def move_by_lat_lon_diff(self, location: "Location") -> Tuple[float, float]:
    return location.latitude - self.latitude_diff, location.longitude + self.longitude_diff
- **strategy**: llm
