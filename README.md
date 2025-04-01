# Ringtone Maker

Ringtone Maker is a command-line tool to create iPhone ringtones from video and audio files.

Transfer the generated files by dragging and dropping them to your device in the Finder, after connecting your iPhone to your Mac.

## Installation

Install with [Homebrew](https://brew.sh):

```shell
brew install vitorgalvao/tiny-scripts/ringtone-maker
```

Alternatively, download the executable at the root of this repository and call it directly. Ensure you have [`ffmpeg`](https://ffmpeg.org) installed and in your `PATH`.

## Usage

```
Convert video and audio files to iPhone ringtones.

Usage:
  ringtone-maker --input <file> --output <file> [--duration <integer>] [--start-time <time>] [--fade-out <integer>] [--play-after]

Options:
  -i, --input <file>         File to convert.
  -o, --output <file>        File to save.
  -d, --duration <integer>   Duration (in seconds) of the output file. Maximum is 40.
  -f, --fade-out <integer>   Duration (in seconds) of audio fade out at the end. Default is 1.
  -s, --start-time <time>    Start time from when to start cutting, in the form xx:xx:xx.
  -p, --play-after           Play ringtone after converting.
  -h, --help                 Show this help.
```

## License

3-Clause BSD
