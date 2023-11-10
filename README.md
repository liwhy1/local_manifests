# local_manifests
Custom manifest for EvoX on tiramisu.

### Sync ###

```bash
# Initialize rom repository
repo init -u https://github.com/Evolution-X/manifest -b tiramisu

# Clone custom manifest
git clone https://github.com/liwhy1/local_manifests -b tiramisu .repo/local_manifests

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash
# Set up environment
source build/envsetup.sh

# Build the code
brunch denniz
```
