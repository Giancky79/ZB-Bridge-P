# ZB-Bridge-P
Sonoff ZB-Bridge-P

only if you want a backup the original bin

python3 -m pip install --upgrade pip
python3 -m pip install esptool

python3 -m esptool

for backup

python3 -m esptool -p /dev/cu.usbserial-1420 read_flash 0x0 0x400000 oem-firmware.bin

for restore

python3 -m esptool -p /dev/cu.usbserial-1420 write_flash 0x0 oem-firmware.bin
