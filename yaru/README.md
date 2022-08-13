# yaru

Home site: https://github.com/ubuntu/yaru/

Full yaru gnome theme

https://github.com/ubuntu/yaru

How to clone this repo:

```
git clone https://gitlab.com/rebornos-team/themes-and-icons/yaru.git
```

NOTE: if makepkg doesn't work, you have to temporarily downgrade **libsass** to
version 3.6.1. To do this, we must install downgrade, and then make the
version change. Let's see the steps:

```
sudo pacman -S downgrade
downgrade libsass

Paquetes disponibles:

   1)  libsass    3.5.5  1  x86_64  (remoto)
   2)  libsass    3.5.5  2  x86_64  (remoto)
   3)  libsass    3.6.0  1  x86_64  (remoto)
   4)  libsass    3.6.1  1  x86_64  (remoto)
   5)  libsass    3.6.2  1  x86_64  (remoto)
+  6)  libsass    3.6.3  1  x86_64  (remoto)
+  7)  libsass    3.6.3  1  x86_64  (local)

Selecciona un paquete por su número: 4
```

It will ask us if we want to add the package to the list of those that will not
be modified in the following updates. We answer **no**.

