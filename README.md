# Gexis Player sample plugins

The two sample plugins from
[*Writing a plugin for Gexis Player*](https://github.com/gcarstoiu/gexis-player/blob/main/docs/WRITING-A-PLUGIN.md),
published as an author publishes a plugin for the
[plugin catalogue](https://github.com/gcarstoiu/gexis-plugins): each version
a `.tar.gz` on a release of this repository.

| Folder | Plugin | What it does |
|---|---|---|
| `hello/` | Hello (sample), a service | Says hello to the player, keeps a file in its own data folder, and writes to the player's log what the sandbox allows and refuses. |
| `tone/` | Tone (sample), a renderer | Adds a source button that plays a quiet 440 Hz tone for 20 seconds. |

## Building

`./package.sh` builds `dist/<id>-<version>.tar.gz` for both, `./package.sh
hello` for one. It packs the files git tracks in that folder, in a fixed
order, owner and date, so the same tag always gives the same bytes and a
listed archive's SHA-256 can be checked against it.

## Releases

One tag per version of a plugin, `<id>-<version>` (such as `hello-0.1.0`),
with that version's archive as its asset.

## Licence

GNU General Public License, version 3 or later ([LICENSE](LICENSE)).
