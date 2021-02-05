TenX
========

<img src="https://github.com/TenX-OS/TenX_docs/blob/master/banner/banner.png?raw=true">

Getting Started
---------------

To get started with Android, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using the TenX trees, use a command like this:

```bash
repo init -u git://github.com/TenX-OS/manifest_TenX -b eleven
```
Then to sync up:
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

Building the source
---------------
```bash
. build/envsetup.sh
lunch aosp_<device>-userdebug
make bacon -j8 (or) brunch <device>
```
Apply for official maintainership [**HERE**](https://forms.gle/apbQYVAQhwxiV7nH7)
