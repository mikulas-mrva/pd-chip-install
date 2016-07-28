## pd-chip-install
Installation instructions for my C.H.I.P. intended to run pure data

# As a root
`adduser mikulas`
`adduser mikulas sudo`
`/etc/ssh/sshd_config`
set
* PermitRootLogin no
* AllowUsers mikulas

`nmtui`
connect to wifi
`exit`

# As mikulas
`sudo apt-get update`
`sudo apt-get upgrade`
to install 'add-apt-repository'
`sudo apt-get install software-properties-common`
`sudo add-apt-repository ppa:nilarimogard/webupd8`
`sudo apt-get update`
?
`sudo apt-get install ap-hotspot`
