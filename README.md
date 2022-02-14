# mpvcam

mpvcam is a simple posix script to play your webcam in mpv without any latency.
The usage is very simple:
* `$ mpvcam` – toggle the default camera (/dev/video0)
* `$ mpvcam <number>` – toggle a chosen camera (/dev/video\<number>)

## Dependencies
1. mpv

## (Un)Installation
### Universal
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Git clone the repository.
* `$ git clone https://github.com/Amarakon55/mpvcam`
2. Change working directory to *mpvcam*.
* `$ cd mpvcam`
3. Install mpvcam using the Makefile
* `# make install`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Change working directory to *mpvcam*.
* `$ cd mpvcam`
2. Uninstall mpvcam using the Makefile
* `# make uninstall`

### Gentoo
#### Installation
##### Latest Git Master (Bleeding Edge)
1. Add my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using [eselect-repository](https://packages.gentoo.org/packages/app-eselect/eselect-repository)
* `# eselect repository add amarlay git https://github.com/Amarakon55/amarlay`
2. Sync my personal [Gentoo overlay](https://github.com/Amarakon55/amarlay) using `emerge`
* `# emerge --sync amarlay`
3. Emerge the mpvcam package
* `# emerge media-video/mpvcam` or `# emerge mpvcam`
#### Uninstallation
##### Latest Git Master (Bleeding Edge)
1. Unmerge the mpvcam package
* `# emerge -c media-video/mpvcam` or `# emerge -c mpvcam`
2. (Optional) Remove my overlay
* `# eselect-repository remove -f amarlay`
3. (Optional) Sync using `emerge`
* `# emerge --sync`
