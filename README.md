# How to use

```bash
mkdir -p .repo/local_manifests
git clone https://github.com/liwhy1/local_manifests -b evox-10 .repo/local_manifests
repo sync -j$(nproc --all)
```
