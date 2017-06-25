Gentoo Portage Overlay for the Brackets-Electron Code Editor
============================================================

Configuration
-------------

```bash
layman -o https://github.com/gbevan/brackets-electron-bin-overlay/raw/master/repository.xml -f -a gbevan-brackets-electron

emerge -v --ask brackets-electron-bin
```

Upgrade
-------

```bash
layman -S

eix-update

emerge -v --ask -u brackets-electron-bin
```

Developer Notes:
----------------

* When releasing new ebuild, run:

        ebuild brackets-electron-bin-?.?.ebuild manifest

  for your new ebuild version, then commit/push.
