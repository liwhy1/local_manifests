# local_manifests
Custom manifest for evox on udc.

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/Evolution-X/manifest -b udc

# Clone this custom manifest
git clone -b udc https://github.com/liwhy1/local_manifests .repo/local_manifests

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

```

### Build ###

```bash

# Set up environment
. build/envsetup.sh

# Build the code
brunch $DEVICE
```
