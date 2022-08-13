# tor-browser

**Before running makepkg, you must do this (as normal user):**

```
$ gpg --auto-key-locate nodefault,wkd --locate-keys torbrowser@torproject.org
```

If you want to update tor-browser from AUR without AUR helpers you can run in a terminal:

```
$ tor-browser -u
```

Tor Browser Bundle: anonymous browsing using Firefox and Tor (international PKGBUILD)

https://www.torproject.org/projects/torbrowser.html

NOTE: If you want to package tor-browser in a different language, please
      set a `TORBROWSER_PKGLANG` envi
      
How to clone this repo:
      
```
git clone https://gitlab.com/rebornos-team/rebornos-packages/browsers/tor-browser.git
```
      
      