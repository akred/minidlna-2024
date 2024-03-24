# minidlna-portable

Minidlna from Linux Mint Software Library is not using the latest version of MiniDLNA (called ReadyMedia), and os not working Linux Mint 21.3.
This repository contains the latest compiled source from https://sourceforge.net/projects/minidlna/
It might work also for Ubuntu 22.04.

## Dependencies for Linux Mint 21: 

```
sudo apt install libid3tag0
```

## Installation

```
sudo -i
crontab -e
```

add this line:

```
@reboot [path-this-folder]/minidlnad -f [path-this-folder]/minidlna.conf
```

Edit minidlna.conf:

```
media_dir=[path-to-your-media-files]
```

## Source

I've got the source code from https://sourceforge.net/projects/minidlna/