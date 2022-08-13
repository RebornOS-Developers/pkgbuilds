# enpass-bin

A multiplatform password manager

http://enpass.io/

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/rebornos-packages/enpass-bin.git
```

To check if there's a new version available:

```
curl -so- https://apt.enpass.io/dists/stable/main/binary-amd64/Packages.gz | zcat | egrep "Package|Version|SHA256" | head -n 3
```

