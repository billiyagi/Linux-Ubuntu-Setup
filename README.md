
# Ubuntu Setup
  Daftar package rekomendasi:
- [Nala Package Manager](https://github.com/billiyagi/Linux-Ubuntu-Setup#nala---package-manager)
- [Tweaks](https://github.com/billiyagi/Linux-Ubuntu-Setup#tweaks)
- [Gnome Ekstension](https://github.com/billiyagi/Linux-Ubuntu-Setup#gnome-ekstension)
- [Flatpak](https://github.com/billiyagi/Linux-Ubuntu-Setup#flatpak)
- [Web Apps](https://github.com/billiyagi/Linux-Ubuntu-Setup#web-apps)
- [XAMPP Control Panel](https://github.com/billiyagi/Linux-Ubuntu-Setup#xampp-control-panel)
- [Wine & Playonlinux](https://github.com/billiyagi/Linux-Ubuntu-Setup#wine--playonlinux)


## Nala - Package manager
Install nala 

```bash
sudo nala update
sudo apt install nala
```

cara penggunaan tetap sama seperti apt hanya diganti menjadi nala

contoh:
```bash
sudo nala install NAMA_PACKAGE
```
## Tweaks
Instalasi

```bash
sudo nala update
sudo nala install gnome-tweaks
```

Download browser integrasi :
[Ekstensi Chrome](https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep?hl=en-US)

## Gnome Ekstension

Install ekstensi di [Gnome Ekstension](https://extensions.gnome.org/)

Download Tema di [Gnome Look](https://www.gnome-look.org/)


Rekomendasi ekstensi: 
- User Themes
- Bluetooth Quick Connect
- Dash to Dock
- GTK Title Bar
- Network Stats
- No activities button
- Search Light
- Transparent Top Bar (Adjustable transparency)
- Unite

Rekomendasi Icon:
- [Kora](https://www.gnome-look.org/p/1256209/)

Rekomendasi Pengembang tema:
- [Vinceliuice](https://www.gnome-look.org/u/vinceliuice)
- [Tarma](https://www.gnome-look.org/u/tarma)

## Flatpak

Instalasi Flatpak
```bash
sudo nala update
sudo nala install flatpak
```


## Web apps
Instalasi Web app manager

```bash
sudo nala update
sudo nala install webapp-manager
```
## XAMPP Control Panel

Pergi ke halaman [Download XAMPP](https://www.apachefriends.org/download.html) lalu download xampp yang terbaru


### Setup xampp
Ganti izin aplikasi

```bash
sudo chmod 755 NAMA_FILE_XAMPP
```

Lalu jalankan installer xampp

```bash
./NAMA_FILE_XAMPP
```

Buat folder htdocs menjadi dapat diakses oleh user mana saja

```bash
sudo chmod 755 /opt/lampp/htdocs
```

Ubah folder htdocs menjadi diluar grup root

```bash
chown NAMA_USER:NAMA_GRUP_USER /opt/lampp/htdocs
```

Buat ikon XAMPP dapat diakses pada menu

```bash
cd ./local/share/applications
nano XAMPP.desktop
```

Pada file XAMPP.desktop paste kode ini

```bash
[Desktop Entry]
Encoding=UTF-8
Name=XAMPP Control Panel
Comment=Start and Stop XAMPP
Exec=sh -c "pkexec env DISPLAY=$DISPLAY XAUTHORITY=$XAUTHORITY /opt/lampp/manager-linux-x64.run"
Icon=/opt/lampp/htdocs/favicon.ico
Categories=Application
Type=Application
Terminal=false
```
## Wine & Playonlinux

Install wine

```bash
sudo nala install wine
```

Install Playonlinux

```bash
sudo nala install playonlinux
```
