# dxlAPRS
dxlAPRS Archives by OE5HPM

Last Update: Aug 27th 2023

This repository contains the dxlAPRS archives from http://dxlaprs.hamspirit.at/
In 2023 the site was down longer time, so I decided to provide the archives here and additionally some "updates".
There are no starting scripts for APRS or radiosonde reception included in the archives, but examples can be downloaded in my other Github repositories.

## References

- Original dxlAPRS Github repository from OE5HPM with sources: https://github.com/oe5hpm/dxlAPRS
- Newer binaries can be found here at the OE5DXL site: http://oe5dxl.hamspirit.at:8025/aprs/bin
- Script for updating the installation with the newest compiled binaries by OE5DXL: https://github.com/dl1nux/dxlAPRS-update
- Scripts for APRS operation: https://github.com/dl1nux/dxlAPRS-APRS-Skripte
- Scripts for radiosonde operation: https://github.com/dl1nux/dxlAPRS-radiosonde-rx
- dxlAPRS Wiki in german language by DL1NUX: https://dxlwiki.dl1nux.de

## Archive files
- `dxlAPRS_armv6-current.tgz` (RaspberryPi 1B or Zero W/H, 32 bit only)
- `dxlAPRS_armv6tce-current.tgz` (Tinycore Linux Edition, 32 bit only)
- `dxlAPRS_armv7hf-current.tgz` (RaspberryPi 2 and up, BananaPi, OrangePi etc., 32bit only)
- `dxlAPRS_x86_32-current.tgz` (Linux x86 PCs, 32 bit)
- `dxlAPRS_x86_64-current.tgz` (Linux X86 PCs, 64 bit)

## Additional files
These files are newer and not included in the archives. Copy them to `/dxlAPRS/aprs/www/`.
- `maplink.txt` : Link for showing stations positions on Openstreetmap (click on callsign package counter in webinterface)
- `objectlink.txt` : Link for Radiosonde APRS Objects in object MH-List (click on object call)
- `style.css` : Optional CSS-File for better readability of the webinterface with bigger fonts

`maplink.txt` and `objectlink.txt` need the newest udpgate4 binary, so make an update after unpacking the archives

## Icon update from DO1TNP
GIF icons created by Thorsten DO1TNP located in `/icon-udpate/*` can be copied to `/dxlAPRS/aprs/www/icon/` and replace the old ones. The old ones are also included for comparison with suffix `_alt`.

## Short installation instructions:

ARMv7:
```
cd ~
wget https://github.com/dl1nux/dxlAPRS/raw/main/dxlAPRS_armv7hf-current.tgz
tar xzvf dxlAPRS_armv7hf-current.tgz --strip=1 scripts/updateDXLaprs
./updateDXLaprs dxlAPRS_armv7hf-current.tgz
```

ARMv6:
```
cd ~
wget https://github.com/dl1nux/dxlAPRS/raw/main/dxlAPRS_armv6-current.tgz
tar xzvf dxlAPRS_armv6-current.tgz --strip=1 scripts/updateDXLaprs
./updateDXLaprs dxlAPRS_armv6-current.tgz
```

Linux x86-64
```
cd ~
wget https://github.com/dl1nux/dxlAPRS/raw/main/dxlAPRS_x86_64-current.tgz
tar xzvf dxlAPRS_x86_64-current.tgz --strip=1 scripts/updateDXLaprs
./updateDXLaprs dxlAPRS_x86_64-current.tgz
```

Linux x86-32
```
cd ~
wget https://github.com/dl1nux/dxlAPRS/raw/main/dxlAPRS_x86_32-current.tgz
tar xzvf dxlAPRS_x86_32-current.tgz --strip=1 scripts/updateDXLaprs
./updateDXLaprs dxlAPRS_x86_32-current.tgz
```

73 de Attila DL1NUX
