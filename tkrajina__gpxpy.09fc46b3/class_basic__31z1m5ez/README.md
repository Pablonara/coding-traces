# Bug Repository: tkrajina__gpxpy.09fc46b3

## Bug Information

- **Bug ID**: class_basic__31z1m5ez
- **Repository**: tkrajina__gpxpy.09fc46b3
- **Strategy**: llm
- **Cost**: 0.00206029

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

- **cost**: 0.00206029
- **output**: ```python
class GPXBounds:
    gpx_10_fields = gpx_11_fields = [
            mod_gpxfield.GPXField('min_latitude', attribute='minlat', type=mod_gpxfield.FLOAT_TYPE),
            mod_gpxfield.GPXField(...
- **rewrite**: class GPXBounds:
    gpx_10_fields = gpx_11_fields = [
            mod_gpxfield.GPXField('min_latitude', attribute='minlat', type=mod_gpxfield.FLOAT_TYPE),
            mod_gpxfield.GPXField('max_latit...
- **strategy**: llm
