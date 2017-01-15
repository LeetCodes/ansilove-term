![Ansilove-Term Example](docs/ansilove-term-bellum.png)

# Description

Ansilove-Term is a command line tool to render text-mode art files as PNG files, as well as displaying in several different mediums.

# Requirements & Building

You may have to update your compiler in order to support `C++11` language features.

Then type:

    make

# Usage

    usage: ans [--version] [--help] [--text] [--ansi] [--xterm256] [--xterm24bit]
           [--png] [file ...] [file ...]
    
    --text                 Display as plain-text
    --ansi                 Display with ANSi escape sequences
    --xterm256             Display with XTerm's 256-color palette
    --xterm24bit           Display with 24-Bit escape sequences
    --png                  Output as PNG


ANSI, AnsiEdit, Artworx, ASCII, Binary, Ice Draw, PCBoard, Tundra, and XBin are supported. All color code sequences are matched with their nearest equivalent using the XTerm-256color palette, so results may vary for files that contain 24-bit color information. For best result, use [BlockZone][1] font.

[LodePNG](https://github.com/lvandeve/lodepng) is used, and already included in the project, for PNG output.

# License

Ansilove is released under the BSD 3-Clause license. See `LICENSE.txt` file for details.

# Author

Ansilove-Term is developed by Andrew Herbert.

[1]: https://github.com/ansilove/BlockZone