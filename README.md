# Brightis (English)

Brightis is a 1999 PlayStation action RPG by Quintet and Shade, the studios
behind Soul Blazer and Terranigma, and it never left Japan. This is an
unofficial English translation patch for it. Everything you read in the game
is in English now: the story, menus, items, skills, the save and load
screens, name entry, signs, area names, and the tutorials.

Version 1.0. It is finished and playable start to finish.

## Download

Grab the latest patch from the [Releases page](../../releases/latest).

You bring your own copy of the game. Please do not ask for it or post it
here. See [CONTRIBUTING.md](CONTRIBUTING.md).

## What you need

- A dump of Brightis (Japan), serial SCPS-10105, that matches the checksums
  below.
- A delta patcher. On Windows, Delta Patcher is the friendly option. On
  macOS or Linux, xdelta3 on the command line does the job.

### The disc this patches

The patch is a delta against the redump.org dump of the original disc
(Redump #9919). Your dump has to match this exactly or the patcher will turn
it away, which is the point: it stops you patching the wrong file.

| Disc     | Serial     | Size (bytes) | CRC32    | MD5                              | SHA-1                                    |
|----------|------------|--------------|----------|----------------------------------|------------------------------------------|
| 1 (only) | SCPS-10105 | 102,319,056  | 7fdab825 | e69e9013df15e4b9625dfca32af2c070 | 94dbbff6ba125b4c155084686e41e1650f6eab41 |

One track, MODE2/2352.

## How to patch

Step by step in [docs/patching-guide.md](docs/patching-guide.md).

## Status

Complete. The full script is translated, along with every menu, all items
and equipment, skills, the save and load UI, name entry, field signs, area
names, and tutorials. A couple of small, deliberate exceptions are listed in
[docs/known-issues.md](docs/known-issues.md).

## Found something wrong?

Reports are genuinely welcome, that is what this repo is for. Open an
[issue](../../issues/new/choose) and give me enough to track it down: where
you were in the game, and a screenshot if you can manage one. Please skim
[CONTRIBUTING.md](CONTRIBUTING.md) first. Short version: this project takes
reports, not code.

## Credits

Translation by Wado.

Built on the groundwork of the original fan-translation team, with thanks:

- D. Debonair (Dickdebonair)
- realonepiecefreak (onepiecefreak3)
- Stewie (fortiersteven)
- Louis-Land

Thanks also to the redump.org preservation project.

## License

This is a fan translation. It is free, not for sale, and not affiliated with
Sony or the original developers. Please support the official release. Full
usage and credit terms are in [LICENSE](LICENSE).
