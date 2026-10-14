# scoop-urna

scoop bucket for [urna](https://github.com/hoffresearch/urna).

```powershell
scoop bucket add hoffresearch https://github.com/hoffresearch/scoop-urna
scoop install urna
urna setup
```

`bucket/urna.json` is written by the `scoopship` job of `hoffresearch/urna` on every tagged release, from that release's own archive and SHA-256; do not edit it by hand. It installs the binary only: `urna setup` lays down the offline embedder and checks the install.
