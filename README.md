# local_manifests
Custom manifest forked from nattolecats.

### Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/Evolution-X/manifest -b tiramisu

# Clone my custom manifest
git clone -b tiramisu https://github.com/liwhy1/local_manifests .repo/local_manifests

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

`brunch` is recommended because my tree contains `vendorsetup.sh` automatic setting up environment. and also for MTK, do patch to source codes. For EvoX, `lunch` triggers running `vendorsetup.sh`. if you're have confidence of don't forget, you can also do `lunch evolution_$DEVICE-userdebug && m evolution` instead.
