# dropbox

A free service that lets you bring your photos, docs, and videos anywhere and share them easily.

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/rebornos-packages/cloud/dropbox.git
```

https://www.dropbox.com


Run the following command in case you got errors during "Verifying source file signatures with gpg..."

```
gpg --recv-keys 1C61A2656FB57B7E4DE0F4C1FC918B335044912E
```

Alternatively, you can download Dropbox's public key from https://linux.dropbox.com/fedora/rpm-public-key.asc and import it with:

```
gpg --import rpm-public-key.asc
```
You can check whether keys are successfully imported or not using the output of gpg -k. You should find something like this:

```
pub   rsa2048 2010-02-11 [SC]
      1C61A2656FB57B7E4DE0F4C1FC918B335044912E
uid           [ unknown] Dropbox Automatic Signing Key <linux@dropbox.com>
```

