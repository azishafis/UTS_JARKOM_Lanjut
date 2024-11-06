# Azis Hafish 2021081141
# UTS_JARKOM_Lanjut

# ESSAY
1. Menurut saya Routing statis adalah dengan mengatur semua rute konfigurasinya dilakukan secara manual.
2. Menurut saya Routing dinamis adalah routing yang dilakukan semua routing konfigurasinya dilakukan secara dinamis atau otomatis sesuai dengan jaringan yang ada
3. Menurut saya firewall adalah sistem keamanan jaringan yang dibuat untuk mengawasi, memfilter, dan mengontrol setiap lalu lintas data yang masuk dan keluar dari suatu jaringan
4. Menurut saya NAT adalah metode yang memungkinkan beberapa perangkat di jaringan lokal terhubung ke internet menggunakan satu alamat IP publik. Penggunaan NAT membantu juga untuk membantu mengatasi keterbatasan alamat IP yang tersedia dan juga memberikan keamanan tambahan bagi jaringan internal


# Cased 

# Topologi
![Blank diagram (1)](https://github.com/user-attachments/assets/529918a9-d95b-4ef6-992e-a71c527ef60f)

# Konfigurasi
1. Router CR:
- IP Publik: 152.167.20.5/24
- IPIP Tunnel ke Router KJ: 30.30.30.1/24
- LAN: 192.168.20.1/24 dengan PC di 192.168.11.2/24
- Rute Statis: Arahkan lalu lintas ke jaringan Router KJ dan KHI melalui tunnel.

2. Router KJ:
- IP Publik: 152.167.10.5/24
- IPIP Tunnel ke Router CR: 30.30.30.2/24
- IPIP Tunnel ke Router KHI: 40.40.40.1/24
- LAN: 192.168.20.2/24 dengan PC di 192.168.12.2/24
- Rute Statis: Arahkan lalu lintas ke jaringan Router CR dan KHI melalui tunnel.

3. Router KHI:
- IP Publik: 152.167.30.5/24
- IPIP Tunnel ke Router KJ: 40.40.40.2/24
- LAN: 192.168.20.3/24 dengan PC di 192.168.13.2/24
- Rute Statis: Arahkan lalu lintas ke jaringan Router CR dan KJ melalui tunnel.
