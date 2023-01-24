<img src="https://user-images.githubusercontent.com/113618658/214139255-c81222c9-48a2-46c9-a509-3e613d390d55.jpg" width="340" height="200" />

# Musort

A Python3 program that renames all selected music/audio files in a folder with a specified naming convention 

## Features

- Rename many audio files at once
- Rename all files in subdirectories as well (recursive)
- Choose the naming convention (ex. track.title.flac or artist.track.year.mp3)
- Give a separator for the naming of the file (ex. track.title.flac or track_title.flac)
- Works on all systems that can run Python


## Demo


## Dependencies
- [Python3](https://www.python.org/)
- [TinyTag](https://pypi.org/project/tinytag/) (Installable from Python Package Index)
## Installation and Usage

Clone the repository and run the Python program

``` Bash
git clone https://github.com/tdeerenberg/Musort.git
cd Musort
pip install requirements.txt
python3 musort.py
```
Alternatively, you could move `musort.py` into a directory in your `$PATH` and rename `musort.py` to `musort`. After that, the program can run like this:
``` Bash
musort music_directory track.title.year -s _ -r
```

## Manual (options and arguments)
```
Musort © 2023 tdeerenberg (github.com/tdeerenberg)

DESCRIPTION:
A Python3 program that renames all selected music/audio files in a folder with a specified naming convention

USAGE:
musort [DIRECTORY] [NAMING_CONVENTION] [OPTIONAL_OPTIONS]...

    USAGE EXAMPLES:
    musort ~/music track.title.year -s _ -r
    musort /local/music disc.artist.title.album -r
    musort ~/my_music track.title

OPTIONAL OPTIONS:
-h, --help           Show the help menu
-s, --separator      Set the separator for the filename (ex. '-s .' -> 01.track.flac and '-s -' -> 01-track.mp3)
                     Default separator ( . ) will be used if none is given
-r, --recursive      Rename files in subdirectories as well

NAMING CONVENTION:
FORMAT_OPTION.FORMAT_OPTION...      The amount of format options does not matter.
                                    It can be one, two, three, even all of them.
                                    (See FORMAT OPTIONS below for all options)

FORMAT OPTIONS:
album           album as string
albumartist     album artist as string
artist          artist name as string
audio_offset    number of bytes before audio data begins
bitdepth        bit depth for lossless audio
bitrate         bitrate in kBits/s
comment         file comment as string
composer        composer as string 
disc            disc number
disc_total      the total number of discs
duration        duration of the song in seconds
filesize        file size in bytes
genre           genre as string
samplerate      samples per second
title           title of the song
track           track number as string
track_total     total number of tracks as string
year            year or date as string
```
## Authors

- [@tdeerenberg](https://www.github.com/tdeerenberg)

## License

[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. 