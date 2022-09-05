# PixysOS

### How to build ###

```bash
# Create dirs
$ mkdir PixysOS && cd PixysOS

# Init repo
$ repo init -u https://github.com/PixysOS/manifest -b ten

# Clone my local repo
$ git clone https://github.com/batuhantrkgl/android_manifest_samsung_j7y17lte.git -b pixysos-staging .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ . build/envsetup.sh && lunch lineage_j7y17lte-userdebug && mka clean && mka api-stubs-docs && mka hiddenapi-lists-docs && mka system-api-stubs-docs && mka test-api-stubs-docs && mka bacon -j`nproc`
```

## Credits
2019 @Astrako
2022 @Batuhantrkgl

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A
