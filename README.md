# wgm

Script for quickly managing Wireguard connections. Shows connection status. Turns the connection on or off.

Usage example:

```bash
$ sudo ./wgm

1) wg0-cloud1 active
2) wg0-cloud2
3) Show stat
4) Exit

Select: 1

[#] ip link delete dev wg0-cloud1
[#] resolvconf -d tun.wg0-cloud1 -f

```

Or add this script into sudoers.

```bash
cp ./wgm /usr/local/bin/wgm

ubuntu ALL=(ALL) NOPASSWD: /usr/local/bin/wgm
```
