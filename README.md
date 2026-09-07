# EXCS Mammoth Gru

Cloning this repo in root should add all of the necessary files automatically, such as `/etc/dnsmasq.conf`.

To clone:

```sh
cd /
git init
git remote add origin https://github.com/EXCS-Project-Mammoth/gru.git
git fetch
git checkout -f main
```

To add a new file it may be necessary to execute `git add -f <PATH>`, particularly if it's in a subfolder.

Other things that need configuring:

- Cloudflared needs installing and running separately. After cloning, update `/etc/systemd/system/cloudflared.service`, filling in the token as needed.
