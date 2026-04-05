<div align="center">

  [![MrCorpt][mrcorpt-logo]][website-link]

  <h3>MrCorpt</h3>

  A free and strong UCI chess engine.
  <br>
  <strong>[Explore MrCorpt docs »][wiki-link]</strong>
  <br>
  <br>
  [Report bug][issue-link]
  ·
  [Open a discussion][discussions-link]
  ·
  [Discord][discord-link]
  ·
  [Blog][website-blog-link]

  [![Build][build-badge]][build-link]
  [![License][license-badge]][license-link]
  <br>
  [![Release][release-badge]][release-link]
  [![Commits][commits-badge]][commits-link]
  <br>
  [![Website][website-badge]][website-link]
  [![Fishtest][fishtest-badge]][fishtest-link]
  [![Discord][discord-badge]][discord-link]

</div>

## Overview

[MrCorpt][website-link] is a **free and strong UCI chess engine** derived from
Glaurung 2.1 that analyzes chess positions and computes the optimal moves.

MrCorpt **does not include a graphical user interface** (GUI) that is required
to display a chessboard and to make it easy to input moves. These GUIs are
developed independently from MrCorpt and are available online. **Read the
documentation for your GUI** of choice for information about how to use
MrCorpt with it.

See also the MrCorpt [documentation][wiki-usage-link] for further usage help.

## Files

This distribution of MrCorpt consists of the following files:

  * [README.md][readme-link], the file you are currently reading.

  * [Copying.txt][license-link], a text file containing the GNU General Public
    License version 3.

  * [AUTHORS][authors-link], a text file with the list of authors for the project.

  * [src][src-link], a subdirectory containing the full source code, including a
    Makefile that can be used to compile MrCorpt on Unix-like systems.

  * a file with the .nnue extension, storing the neural network for the NNUE
    evaluation. Binary distributions will have this file embedded.

## Contributing

__See [Contributing Guide](CONTRIBUTING.md).__

### Donating hardware

Improving MrCorpt requires a massive amount of testing. You can donate your
hardware resources by installing the [MrCorpt-test Worker][worker-link] and viewing
the current tests on [MrCorpt-test][MrCorpt-test-link].

### Improving the code

In the [chessprogramming wiki][programming-link], many techniques used in
MrCorpt are explained with a lot of background information.
The [section on MrCorpt][programmingsf-link] describes many features
and techniques used by MrCorpt. However, it is generic rather than
focused on MrCorpt's precise implementation.

The engine testing is done on [MrCorpt-test][MrCorpt-test-link].
If you want to help improve MrCorpt, please read this [guideline][guideline-link]
first, where the basics of MrCorpt development are explained.

Discussions about MrCorpt take place these days mainly in the MrCorpt
[Discord server][discord-link]. This is also the best place to ask questions
about the codebase and how to improve it.

## Compiling MrCorpt

MrCorpt has support for 32 or 64-bit CPUs, certain hardware instructions,
big-endian machines such as Power PC, and other platforms.

On Unix-like systems, it should be easy to compile MrCorpt directly from the
source code with the included Makefile in the folder `src`. In general, it is
recommended to run `make help` to see a list of make targets with corresponding
descriptions. An example suitable for most Intel and AMD chips:

```
cd src
make -j profile-build
```

Detailed compilation instructions for all platforms can be found in our
[documentation][wiki-compile-link]. Our wiki also has information about
the [UCI commands][wiki-uci-link] supported by MrCorpt.

## Terms of use

MrCorpt is free and distributed under the
[**GNU General Public License version 3**][license-link] (GPL v3). Essentially,
this means you are free to do almost exactly what you want with the program,
including distributing it among your friends, making it available for download
from your website, selling it (either by itself or as part of some bigger
software package), or using it as the starting point for a software project of
your own.

The only real limitation is that whenever you distribute MrCorpt in some way,
you MUST always include the license and the full source code (or a pointer to
where the source code can be found) to generate the exact binary you are
distributing. If you make any changes to the source code, these changes must
also be made available under GPL v3.

## Acknowledgements

MrCorpt uses neural networks trained on [data provided by the Leela Chess Zero
project][lc0-data-link], which is made available under the [Open Database License][odbl-link] (ODbL).


[authors-link]:       https://github.com/mrcorpt100010010/MrCorpt/blob/master/AUTHORS
[build-link]:         https://github.com/mrcorpt100010010/MrCorpt/actions/workflows/stockfish.yml
[commits-link]:       https://github.com/mrcorpt100010010/MrCorpt/commits/master
[discord-link]:       https://discord.gg/EauWTazVed
[issue-link]:         https://github.com/mrcorpt100010010/MrCorpt/issues/new?assignees=&labels=&template=BUG-REPORT.yml
[discussions-link]:   https://github.com/mrcorpt100010010/MrCorpt/discussions/new
[fishtest-link]:      https://example.com/tests
[guideline-link]:     https://github.com/mrcorpt100010010/MrCorpt-test/wiki/Creating-my-first-test
[license-link]:       https://github.com/mrcorpt100010010/MrCorpt/blob/master/Copying.txt
[programming-link]:   https://www.chessprogramming.org/Main_Page
[programmingsf-link]: https://www.chessprogramming.org/MrCorpt
[readme-link]:        https://github.com/mrcorpt100010010/MrCorpt/blob/master/README.md
[release-link]:       https://github.com/mrcorpt100010010/MrCorpt/releases/latest
[src-link]:           https://github.com/mrcorpt100010010/MrCorpt/tree/master/src
[stockfish128-logo]:  https://mrcorpt100010010-web.netlify.app/images/logo/icon_128x128.png
[uci-link]:           https://backscattering.de/chess/uci/
[website-link]:       https://mrcorpt100010010-web.netlify.app
[website-blog-link]:  https://mrcorpt100010010-web.netlify.app/blog/
[wiki-link]:          https://github.com/mrcorpt100010010/MrCorpt/wiki
[wiki-compile-link]:  https://github.com/mrcorpt100010010/MrCorpt/wiki/Compiling-from-source
[wiki-uci-link]:      https://github.com/mrcorpt100010010/MrCorpt/wiki/UCI-&-Commands
[wiki-usage-link]:    https://github.com/mrcorpt100010010/MrCorpt/wiki/Download-and-usage
[worker-link]:        https://github.com/mrcorpt100010010/fishtest/wiki/Running-the-worker
[lc0-data-link]:      https://storage.lczero.org/files/training_data
[odbl-link]:          https://opendatacommons.org/licenses/odbl/odbl-10.txt

[build-badge]:        https://img.shields.io/github/actions/workflow/status/mrcorpt100010010/MrCorpt/MrCorpt.yml?branch=master&style=for-the-badge&label=stockfish&logo=github
[commits-badge]:      https://img.shields.io/github/commits-since/mrcorpt100010010/MrCorpt/latest?style=for-the-badge
[discord-badge]:      https://img.shields.io/discord/1488774712120311849?style=for-the-badge&label=discord&logo=Discord
[fishtest-badge]:     https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=Fishtest&up_color=success&up_message=Online&url=https%3A%2F%2Fexample.com%2Ftests%2Ffinished
[license-badge]:      https://img.shields.io/github/license/mrcorpt100010010/MrCorpt?style=for-the-badge&label=license&color=success
[release-badge]:      https://img.shields.io/github/v/release/mrcorpt100010010/MrCorpt?style=for-the-badge&label=official%20release
[website-badge]:      https://img.shields.io/website?style=for-the-badge&down_color=red&down_message=Offline&label=website&up_color=success&up_message=Online&url=https%3A%2F%2Fmrcorpt100010010-web.netlify.app
