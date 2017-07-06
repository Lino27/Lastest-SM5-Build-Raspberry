# Lastest-SM5-Build-Raspberry
Método simples de build do Stepmania 5 no Raspberry Pi 3

0. install gcc / g++
1. sudo apt-get install cmake gcc g++ libmad0-dev libgtk2.0-dev binutils-dev git-core make libasound2-dev yasm libc6-dev libogg-dev libvorbis-dev libbz2-dev zlib1g-dev libjpeg8-dev libpng12-dev libxtst-dev libxrandr-dev libglew-dev libglu1-mesa-dev mesa-common-dev automake autoconf libva-dev libjack-dev
2. git clone https://github.com/stepmania/stepmania.git
3. git submodule update --init
4. cmake '/home/pi/stepmania' -DCMAKE_INSTALL_PREFIX='/home/pi/sm5-run' -DWITH_FFMPEG=1 -DWITH_MINIMAID=0 -DWITH_CRASH_HANDLER=0 -DWITH_SSE2=0 -DWITH_FULL_RELEASE=1 -DWITH_TEXTURE_GENERATOR=0 -DWITH_GLES2=0 && make install -j4 && sync

1. from sm5 github (debian)
sudo apt-get install build-essential
sudo apt-get install mesa-common-dev libglu1-mesa-dev libglew1.5-dev libxtst-dev libxrandr-dev libpng12-dev libjpeg-dev zlib1g-dev libbz2-dev libogg-dev libvorbis-dev libc6-dev yasm libasound-dev libpulse-dev binutils-dev libgtk2.0-dev libmad0-dev libudev-dev libva-dev
