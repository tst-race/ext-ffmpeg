# FFmpeg for RACE

This repo provides scripts to custom-build the
[FFmpeg tool](https://ffmpeg.org/) for RACE.

## License

The FFmpeg tool is licensed under the GPL license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

FFmpeg has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build FFmpeg.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-ffmpeg.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-ffmpeg
```

## Platforms

FFmpeg is built for the following platforms:

* `linux-x86_64`
* `linux-arm64-v8a`

## How It Is Used

FFmpeg is used by the <TO-BE-NAMED> plugin.
