# pd-chip-install
Installation instructions for my C.H.I.P. intended to run pure data

## As root

`adduser mikulas`

`adduser mikulas sudo`

`/etc/ssh/sshd_config`

set

* PermitRootLogin no

* AllowUsers mikulas


`nmtui`

connect to wifi

`exit`

## As mikulas

`sudo apt-get update`

`sudo apt-get upgrade`

to install 'add-apt-repository'

`sudo apt-get install software-properties-common`

`sudo add-apt-repository ppa:nilarimogard/webupd8`

`sudo apt-get update`

?

`sudo apt-get install ap-hotspot`

## test sound

`aplay /usr/share/sounds/alsa/Side_Right.wav`

## install PD-L20rk

[http://l2ork.music.vt.edu/main/make-your-own-l2ork/software/raspberry-pi/]

`wget http://l2ork.music.vt.edu/data/pd/pd-l2ork-armv6l-20160614.deb`

`sudo dpkg -i pd-l2ork*deb`

`sudo apt-get update`

`sudo apt-get -f install`

## RUN PD

`pd -alsa -nogui -audiooutdev "4" -audioindev "3" ./test_in_feedback.pd`

`pd -r 48000 -nogui -audiooutdev "4" -audioindev "4" ./test_in_feedback.pd`

`pd -r 48000 -nogui -audiooutdev "4" -audioindev "4" ./test_in_feedback.pd & alsamixer`
