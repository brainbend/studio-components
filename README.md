# BrainBend Studio components

Downloadable parts of [BrainBend Studio](https://github.com/brainbend/studio) that are not built into the app.
Studio fetches them the first time a feature needs one, checks each file against a published SHA-256, and keeps it in
its own data folder. You never need to download anything here by hand.

## ffmpeg

Used for the still picture of a video and for **Publish as video**. Each release of this repo (`ffmpeg-<version>`)
holds one build per platform and a `manifest.json` listing the file names and their SHA-256 values.

| Platform | Build |
|---|---|
| Windows (x64) | BtbN/FFmpeg-Builds, GPL build |
| Linux (x64) | BtbN/FFmpeg-Builds, GPL build |
| macOS (Intel; runs under Rosetta on Apple silicon) | evermeet.cx static build |

**License.** These are builds of FFmpeg licensed under the GNU General Public License version 3 (`COPYING.GPLv3`).
Studio runs the program as a separate process; it is not linked into Studio, which keeps its own license. Each
platform folder in a release also carries `SOURCE.txt`, which names the exact upstream build and where its source is.

**Source offer.** On request, BrainBend gives anyone who received one of these builds the complete corresponding source
code of the FFmpeg build and the libraries linked into it, for at least three years from the day they received it.
Open an issue in this repository to ask.

H.264 and AAC are patented formats in some countries. The author of each lesson is responsible for using them where
that is allowed.

This repository contains no code of its own, only these notices and the manifest.
