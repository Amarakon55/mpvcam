mpvcam
================

## Contents

-   [Usage](#usage)
-   [Dependencies](#dependencies)
-   [Installation](#installation)
    -   [Universal](#universal)
    -   [Gentoo](#gentoo)
-   [Uninstallation](#uninstallation)
    -   [Universal](#universal-1)
    -   [Gentoo](#gentoo-1)

mpvcam is a simple posix script to play your webcam in mpv without any
latency.

## Usage

    `# user` mpvcam # toggle the default camera (/dev/video0)
    `# user` mpvcam <number> # toggle a chosen camera (/dev/video\<number>)

## Dependencies

1.  mpv

## Installation

### Universal

``` sh
`# user` git clone https://github.com/amarakon/mpvcam
`# user` cd mpvcam
`# root` make install
```

### Gentoo

``` sh
`# root` eselect repository add amarlay git https://github.com/amarakon/amarlay
`# root` emerge --sync amarlay
`# root` emerge media-video/mpvcam
```

## Uninstallation

### Universal

``` sh
`# user` cd mpvcam
`# root` make uninstall
```

### Gentoo

``` sh
`# root` emerge -c media-video/mpvcam
# Remove my overlay (optional)
`# root` eselect-repository remove -f amarlay
`# root` emerge --sync
```
