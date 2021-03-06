# FFmpeg + nvenc build script

This script will compile FFmpeg with Nvidia NVENC support enabled.
It can also build OBS Studio or Simple Screen Recorder using that FFmpeg build
thus providing NVENC for OBS.

It is brought to you by [Linux GameCast](http://linuxgamecast.com/) and
[Lutris](https://lutris.net) #lgccares

## Requirements

* CUDA driver and toolkit
```
wget http://developer.download.nvidia.com/compute/cuda/10.2/Prod/local_installers/cuda_10.2.89_440.33.01_linux.run
sudo sh cuda_10.2.89_440.33.01_linux.run
```
* unzip
* git


## Usage

Clone the repo then use the `build.sh` script to compile the binaries

```
git clone https://github.com/nicholas-littlelives/ffmpeg-nvenc.git
cd ffmpeg-nvenc
./build.sh --dest $HOME/apps/ffmpeg-nvenc
```

The following command line options are available:

* -d / --dest <path> : Destination path for FFmpeg / OBS
* -o / --obs : Build OBS Studio
* -h / --help : Usage

## TODO

* Add support for multiple distributions (currently only tested on Ubuntu 16.04)

## Supporting the authors

If you find this script useful, you can consider
supporting [Linux GameCast](https://www.patreon.com/linuxgamecast)
and [Lutris](https://www.patreon.com/lutris).
