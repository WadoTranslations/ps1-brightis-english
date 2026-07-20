# Patching guide

This takes about five minutes. You need your own dump of Brightis (Japan) and
the patch from the [Releases page](../../releases/latest).

## 1. Check your disc first

The patch only works on the exact redump.org dump (Redump #9919). Before you
do anything else, confirm your file matches:

- Size: 102,319,056 bytes
- Serial: SCPS-10105
- CRC32: `7fdab825`
- MD5: `e69e9013df15e4b9625dfca32af2c070`
- SHA-1: `94dbbff6ba125b4c155084686e41e1650f6eab41`

If your `.bin` does not match, this patch will not apply to it, and that is
working as intended. A good patcher checks this for you and refuses a wrong
file rather than making a broken game.

## 2. Apply the patch

### Windows (easy way)

Use [Delta Patcher](https://github.com/marcrobledo/RomPatcher.js) or the
desktop Delta Patcher tool.

1. Original file: your `Brightis (Japan).bin`.
2. XDelta patch: the `.xdelta` file from the release.
3. Apply. Rename the result to `Brightis (Japan) [En-v1.0].bin` and keep the
   included `.cue` next to it.

### macOS or Linux (command line)

Install `xdelta3` (Homebrew: `brew install xdelta`, Debian/Ubuntu:
`apt install xdelta3`), then:

```
xdelta3 -d -s "Brightis (Japan).bin" \
    "Brightis (Japan) [En-v1.0].xdelta" \
    "Brightis (Japan) [En-v1.0].bin"
```

## 3. Confirm the result

A clean patch produces a file that is still 102,319,056 bytes, with:

- CRC32: `3a2f5773`
- MD5: `d9949e36c46bf0bf7dfac11f2190594a`
- SHA-1: `53c3935822a528722e3a8732fa8d7c174407b2bc`

If those match, you are done.

## 4. Play it

Put the patched `.bin` and its `.cue` in the same folder and load the `.cue`
in your emulator, or take it to real hardware however you normally would.
Settings and tested setups are in [compatibility.md](compatibility.md).

## A note on the download itself

The release also ships checksums for the patch file. If patching fails and
your source disc is definitely correct, verify the `.xdelta` download against
those first. A half-finished download is a common culprit.
