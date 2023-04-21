```bash
cd /tmp || exit 1
# working directory of your choice
wget https://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz # or curl instead of wget
zcat < install-tl-unx.tar.gz | tar xf -
cd install-tl-* || exit 1
perl ./install-tl --no-interaction # as root or with writable destination
```
Finally, prepend `/usr/local/texlive/YYYY/bin/PLATFORM` to your `PATH`,
e.g., `/usr/local/texlive/2023/bin/x86_64-linux`
