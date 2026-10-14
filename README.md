# scoop-urna

scoop bucket for [urna](https://github.com/hoffresearch/urna).

```powershell
scoop bucket add hoffresearch https://github.com/hoffresearch/scoop-urna
scoop install urna
urna setup
```

`bucket/urna.json` is written by the `scoopship` job of `hoffresearch/urna` on every tagged release, from that release's own archive and SHA-256; do not edit it by hand. It installs the binary only: `urna setup` lays down the offline embedder and checks the install.

What a clean Windows runner prints, from the install test of v0.5.6 (the `scoop windows-latest` leg of `setuptest.yml`):

```text
The hoffresearch bucket was added successfully.
Installing 'urna' (0.5.6) [64bit] from 'hoffresearch' bucket
Downloading https://github.com/hoffresearch/urna/releases/download/v0.5.6/urna-x86_64-pc-windows-msvc.zip (1.8 MB)...
Checking hash of urna-x86_64-pc-windows-msvc.zip... OK.
Extracting urna-x86_64-pc-windows-msvc.zip... Done.
Linking ~\scoop\apps\urna\current => ~\scoop\apps\urna\0.5.6
Creating shim for 'urna'.
'urna' (0.5.6) was installed successfully!

> urna setup
  urna               0.5.6 · x86_64-windows
  channel            scoop · …
  update             scoop update urna
```
