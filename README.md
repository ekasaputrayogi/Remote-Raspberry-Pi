### REMOTE Raspberry Pi 3 
Remote Raspberry Pi 3 dari windows menggunakan SSH dan VNC\

#### Via SSH
* Download Putty
```
https://www.putty.org/
```
* install Putty
* Konek Raspberry pada wifi dan aktifkan mode ssh
- Buka SD card raspberry, lalu pasang pada pada windows menggunakan card reader
- buka directory boot raspberry
- buat file wpa_supplicant.conf, dengan isi file:
```
country=US # Your 2-digit country code
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
network={
    ssid="YOUR_NETWORK_NAME"
    psk="YOUR_PASSWORD"
    key_mgmt=WPA-PSK
}
```
- buat file kosong dengan nama 'ssh' pada directory boot
- pasang kembali SD card pada Raspberry pi
* Setelah raspberry terhubung ke wifi, cari ip adress raspberry menggunakan advance ip scanner
```
https://www.advanced-ip-scanner.com/
```
* Buka putty, masukan ip adress raspberry lalu klik open
* masukan username: pi, password: raspberry

#### VIA VNCS
