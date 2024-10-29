[![Copr Build Status](https://copr.fedorainfracloud.org/coprs/larvitz/throttled/package/throttled/status_image/last_build.png)](https://copr.fedorainfracloud.org/coprs/larvitz/throttled/)

# RPM Package: throttled

This repository holds the RPM package source for [throttled](https://github.com/erpalma/throttled).

## Usage
You can use this package by enabling the copr repository at [larvitz/throttled](https://copr.fedorainfracloud.org/coprs/larvitz/throttled/) as described [here](https://fedorahosted.org/copr/wiki/HowToEnableRepo).

```sh
dnf copr enable larvitz/throttled
dnf copr install throttled
```

### Activation
The package also installs a [systemd.unit](https://www.freedesktop.org/software/systemd/man/systemd.unit.html) file. Which can be activated as shown below.

```sh
systemctl enable --now throttled
```

> **Note:** The configuration used is installed at /etc/throttled.conf
