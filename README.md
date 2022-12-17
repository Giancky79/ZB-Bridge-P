# ZB-Bridge-P
Sonoff ZB-Bridge-P

python3 -m pip install --upgrade pip
python3 -m pip install esptool

python3 -m esptool

python3 -m esptool -p /dev/cu.usbserial-1420 read_flash 0x0 0x400000 oem-firmware.bin


python3 -m esptool -p /dev/cu.usbserial-1420 write_flash 0x0 oem-firmware.bin
