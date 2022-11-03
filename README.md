# CEH
CEH My Tools
Install  PRET 

- Download PRET
- pip install colorama pysnmp
- pip install win_unicode_console
- apt-get install imagemagick ghostscript
- Usage

usage: pret.py [-h] [-s] [-q] [-d] [-i file] [-o file] target {ps,pjl,pcl}

positional arguments:
  target                printer device or hostname
  {ps,pjl,pcl}          printing language to abuse

optional arguments:
  -h, --help            show this help message and exit
  -s, --safe            verify if language is supported
  -q, --quiet           suppress warnings and chit-chat
  -d, --debug           enter debug mode (show traffic)
  -i file, --load file  load and run commands from file
  -o file, --log file   log raw data sent to the target
Example usage:

$ ./pret.py laserjet.lan ps
$ ./pret.py /dev/usb/lp0 pjl
