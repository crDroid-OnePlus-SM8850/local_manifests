# local_manifests - crDroid for OnePlus SM8850

Devices: `infiniti` (OnePlus 15), `fairlady` (OnePlus 15T), `macan` (OnePlus 15R), `macanc` (OnePlus Ace 6T).

```
repo init -u https://github.com/crdroidandroid/android.git -b 17.0 --git-lfs
git clone https://github.com/crDroid-OnePlus-SM8850/local_manifests .repo/local_manifests -b 17.0
repo sync -c -j8
. build/envsetup.sh
brunch <macan|macanc|infiniti|fairlady> [user|userdebug]
```

Vendor repos use Git LFS (`.lfsconfig` points at the LFS server); install `git-lfs` before syncing.
