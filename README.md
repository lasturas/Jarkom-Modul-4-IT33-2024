# Write Up Jarkom Modul 4 Kelompok IT33

| Nama | NRP |
|----------|----------|
| Ricko Mianto Jaya Saputra | 5027231031 |
| Tsaldia Hukma Cita | 5027231036 | 

# Daftar Isi
1. [GNS](#gns)
   - [Topology](#topology-gns)
   - [Pembagian Subnet](#pembagian-subnet-gns)
      - [Gabungan-1](#gabungan-1)
      - [Gabungan-2](#gabungan-2) 
      - [Gabungan-3](#gabungan-3)
      - [Gabungan-4](#gabungan-4)
      - [Gabungan-5](#gabungan-5)
      - [Gabungan-6](#gabungan-6)
      - [Gabungan-7](#gabungan-7)
      - [Gabungan-8](#gabungan-8)
      - [Gabungan-9](#gabungan-9)
      - [Gabungan-10](#gabungan-10)
   - [Tabel Penggabungan](#tabel-penggabungan)
   - [Tree GNS](#tree-gns)
   - [Pembagian IP GNS](#pembagian-ip-gns)
2. [Cisco Packet Tracker](#cisco-packet-tracker)
   - [Topology](#topology-cpt)
   - [Rute](#rute)
   - [Pembagian Area Subnet](#pembagian-area-subnet)
   - [Pembagian IP](#pembagian-ip)
   - [Tree](#tree)

# Sheets IP
Untuk seluruh data dan tabel yang ada di repo ini dapat dilihat di dalam [link](https://docs.google.com/spreadsheets/d/1CGjlsSmBJOj25mW5FXu7kipPXtMJE57o6BJfyq0m8hg/edit?gid=580767165#gid=580767165) berikut 

# GNS
Pada GNS ini kami menggunakan `CIDR`
## Topology GNS
![RUTE](https://github.com/user-attachments/assets/6ba5e34f-0140-4f4e-8575-3f9cc83a8f68)

## Pembagian Subnet GNS
![subnet](https://github.com/user-attachments/assets/a17fc0cf-e8f3-458a-a4a0-96cfec686cd5)

## Gabungan 1
![gabungan 1](https://github.com/user-attachments/assets/755b9e6e-29e8-4240-9cda-74948547ee24)
![image](https://github.com/user-attachments/assets/e999e14c-e567-46d4-b4f3-4e51d68b8f7a)

## Gabungan 2
![gabungan 2](https://github.com/user-attachments/assets/64c8c8cb-b45b-4086-a70f-d09b5605c744)
![image](https://github.com/user-attachments/assets/42a1af87-6633-431a-9d70-d963a90afbcb)

## Gabungan 3
![gabungan 3](https://github.com/user-attachments/assets/72e9803d-eb53-4eeb-bf03-401c0e9751bd)
![image](https://github.com/user-attachments/assets/76556dcf-b816-4c35-a06d-ecf296766e1b)

## Gabungan 4
![gabungan 4 revisi](https://github.com/user-attachments/assets/ab8391b1-dc19-491f-ac4f-8e8f1d2672d1)
![image](https://github.com/user-attachments/assets/890db2e6-0a72-48f0-a5b3-5db7a59168cf)

## Gabungan 5
![gabungan 5 revisi](https://github.com/user-attachments/assets/150123e6-4c46-4601-8d3c-132f72b8ead8)
![image](https://github.com/user-attachments/assets/44a20e1e-13ef-4195-889a-f6f88353565c)

## Gabungan 6
![gabungan 6 revisi](https://github.com/user-attachments/assets/da2cd6a0-b563-4e8e-bcb3-d8952e2be862)
![image](https://github.com/user-attachments/assets/2a07057f-5258-4ff1-a4cd-3e91dbbd56f4)

## Gabungan 7
![gabungan 7 revisi](https://github.com/user-attachments/assets/33fca1f0-7d67-4b9a-b27b-15fa2ab9a846)   
![image](https://github.com/user-attachments/assets/4c0d492c-81c4-4aba-9b91-0d8398443159)

## Gabungan 8
![gabungan 8 revisi](https://github.com/user-attachments/assets/868b82b9-da94-48db-9196-7a7e50a9cd6c)
![image](https://github.com/user-attachments/assets/8443464b-77b7-493b-ae82-ed26cad985a2)

## Gabungan 9
![gabungan 9 revisi](https://github.com/user-attachments/assets/36d8a8a3-78a8-4cc5-a368-c9cc65223fbf)   
![image](https://github.com/user-attachments/assets/01e559c7-2213-43fb-b656-15d1b7cdc479)

## Gabungan 10
![gabungan 10 revisi](https://github.com/user-attachments/assets/cfe5ccf1-5ba7-4210-9a7a-2e24d9a379b2)   
![image](https://github.com/user-attachments/assets/2edb4500-cddd-4a50-9ad8-496ed48e215d)


## Tabel Penggabungan    
![image](https://github.com/user-attachments/assets/96958d84-2cff-4143-946b-90f89c67f63b)

## Tree GNS
![TREE JARKOM 4(SHE)](https://github.com/user-attachments/assets/6244b481-7c34-4bc1-8e69-eea57b7fd02b)

## Pembagian IP GNS
![image](https://github.com/user-attachments/assets/a01afe80-ccf1-45b3-b007-39956e170e4b)

## Config GNS
• Hololive (Gateway)
```
#A15
auto eth1
iface eth1 inet static
    address 192.234.16.1
    netmask 255.255.255.252

#A1
auto eth2
iface eth2 inet static
    address 192.233.160.1
    netmask 255.255.255.252

#A8
auto eth3
iface eth3 inet static
    address 192.233.64.1
    netmask 255.255.255.252
```

• Holo-EN (Gateway)
```
#A15
auto eth0
iface eth0 inet static
    address 192.234.16.2
    netmask 255.255.255.252
    gateway 192.234.16.1

#A18
auto eth1
iface eth1 inet static
    address 192.234.4.1
    netmask 255.255.255.252

#A16
auto eth2
iface eth2 inet static
    address 192.234.8.33
    netmask 255.255.255.252
```

• Holo-Myth (Gateway)
```
#A18
auto eth0
iface eth0 inet static
    address 192.234.4.2
    netmask 255.255.255.252
    gateway 192.234.4.1

#A19
auto eth1
iface eth1 inet static
    address 192.234.0.1
    netmask 255.255.254.0


#A20
auto eth2
iface eth2 inet static
    address 192.234.2.129
    netmask 255.255.255.248
```

• Gura_Ame_Ina (Client)
```
#A19
auto eth0
iface eth0 inet static
    address 192.234.0.2
    netmask 255.255.254.0
    gateway 192.234.0.1
```

• Kiara_Calli (Client)
```
#A19
auto eth0
iface eth0 inet static
    address 192.234.0.3
    netmask 255.255.254.0
    gateway 192.234.0.1
```

• Holo Advent (Gateway)
```
#A16
auto eth0
iface eth0 inet static
    address 192.234.8.34
    netmask 255.255.255.252
    gateway 192.234.8.33

#A17
auto eth1
iface eth1 inet static
    address 192.234.8.1
    netmask 255.255.255.224
```

• FuwaMoco (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.234.8.2
    netmask 255.255.255.224
    gateway 192.234.8.1
```

• Shiori_Nerissa (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.234.8.3
    netmask 255.255.255.224
    gateway 192.234.8.1
```

• Biboo (Client)
```
#A17
auto eth0
iface eth0 inet static
    address 192.234.8.4
    netmask 255.255.255.224
    gateway 192.234.8.1
```

• Project-Hope (Gateway)
```
#A20
auto eth0
iface eth0 inet static
    address 192.234.2.130
    netmask 255.255.255.248
    gateway 192.234.2.129

#A21
auto eth1
iface eth1 inet static
    address 192.234.2.65
    netmask 255.255.255.248
```

• Irys (Client)
```
#A21
auto eth0
iface eth0 inet static
    address 192.234.2.66
    netmask 255.255.255.248
    gateway 192.234.2.65
```

• Holo-Council (Gateway)
```
#A20
auto eth0
iface eth0 inet static
    address 192.234.2.131
    netmask 255.255.255.248
    gateway 192.234.2.130

#A22
auto eth1
iface eth1 inet static
    address 192.234.2.1
    netmask 255.255.255.192
```

• Kronii_Mumei (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.234.2.2
    netmask 255.255.255.192
    gateway 192.234.2.1
```

• Bae_Fauna (Client)
```
#A22
auto eth0
iface eth0 inet static
    address 192.234.2.3
    netmask 255.255.255.192
    gateway 192.234.2.1
```

• Holo-ID (Gateway)
```
#A1
auto eth0
iface eth0 inet static
    address 192.233.160.2
    netmask 255.255.255.252

#A2
auto eth1
iface eth1 inet static
    address 192.233.132.1
    netmask 255.255.255.252

#A4
auto eth2
iface eth2 inet static
    address 192.233.144.65
    netmask 255.255.255.252

#A6
auto eth3
iface eth3 inet static
    address 192.233.130.1
    netmask 255.255.255.252
```

• AREA15 (Gateway)
```
#A2
auto eth0
iface eth0 inet static
    address 192.233.132.2
    netmask 255.255.255.252
    gateway 192.233.132.1

#A3
auto eth1
iface eth1 inet static
    address 192.233.128.1
    netmask 255.255.252.0
```

• Risu (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.233.128.4
    netmask 255.255.252.0
    gateway 192.233.128.1
```

• Moona (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.233.128.3
    netmask 255.255.252.0
    gateway 192.233.128.1
```

• Iofi (Client)
```
#A3
auto eth0
iface eth0 inet static
    address 192.233.128.2
    netmask 255.255.252.0
    gateway 192.233.128.1
```

• Holoro (Gateway)
```
#A4 
auto eth0 
iface eth0 inet static 
      address 192.233.144.66
      netmask 255.255.255.252
      gateway 192.233.144.65

#A5 
auto eth1
iface eth1 inet static 
      address 192.233.144.1
      netmask 255.255.255.192
```

• Ollie (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.233.144.2
    netmask 255.255.255.192
    gateway 192.233.144.1
```

• Anya (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.233.144.3
    netmask 255.255.255.192
    gateway 192.233.144.1
```

• Reine (Client)
```
#A5
auto eth0
iface eth0 inet static
    address 192.233.144.4
    netmask 255.255.255.192
    gateway 192.233.144.1
```

• Holoh3ro (Gateway)
```
#A6
auto eth0
iface eth0 inet static
    address 192.233.130.2
    netmask 255.255.255.252
    gateway 192.233.130.1

#A7
auto eth1
iface eth1 inet static
    address 192.233.136.1
    netmask 255.255.254.0
```

• Zeta (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.233.136.2
    netmask 255.255.254.0
    gateway 192.233.136.1
```

• Kaela (Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.233.136.3
    netmask 255.255.254.0
    gateway 192.233.136.1
```

• Kobo(Client)
```
#A7
auto eth0
iface eth0 inet static
    address 192.233.136.4
    netmask 255.255.254.0
    gateway 192.233.136.1
```

• Holo-JP (Gateway)
```
#A8
auto eth0
iface eth0 inet static
    address 192.233.64.2
    netmask 255.255.255.252
    gateway 192.233.64.1

#A9
auto eth1
iface eth1 inet static
    address 192.233.32.1
    netmask 255.255.255.248
```

• DEV_IS (Gateway)
```
#A9
auto eth0
iface eth0 inet static
    address 192.233.32.2
    netmask 255.255.255.248
    gateway 192.233.32.1

#A10
auto eth1
iface eth1 inet static
    address 192.233.16.1
    netmask 255.255.255.240
```

• Ririka_Raden (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 192.233.16.2
    netmask 255.255.255.240
    gateway 192.233.16.1
```

• Ao (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 192.233.16.3
    netmask 255.255.255.240
    gateway 192.233.16.1
```

• Hajime_Kanade (Client)
```
#A10
auto eth0
iface eth0 inet static
    address 192.233.16.4
    netmask 255.255.255.240
    gateway 192.233.16.1
```

• GEN:0 (Gateway)
```
#A9
auto eth0
iface eth0 inet static
    address 192.233.32.3
    netmask 255.255.255.248
    gateway 192.233.32.1

#A11
auto eth1
iface eth1 inet static
    address 192.233.0.1
    netmask 255.255.248.0
```

• MiComet (Client)
```
#A11
auto eth0
iface eth0 inet static
    address 192.233.0.2
    netmask 255.255.248.0
    gateway 192.233.0.1
```

• Sora_Robo_AZKi (Client)
```
#A11
auto eth0
iface eth0 inet static
    address 192.233.0.3
    netmask 255.255.248.0
    gateway 192.233.0.1
```

• GEN:1 (Gateway)
```
#A11
auto eth0
iface eth0 inet static
    address 192.233.0.4
    netmask 255.255.248.0
    gateway 192.233.0.1

#A14
auto eth1
iface eth1 inet static
    address 192.233.8.1
    netmask 255.255.254.0

#A12
auto eth2
iface eth2 inet static
    address 192.233.10.129
    netmask 255.255.255.252
```

• FBK_Matsuri (Client)
```
#A14
auto eth0
iface eth0 inet static
    address 192.233.8.2
    netmask 255.255.248.0
    gateway 192.233.8.1
```

• Aki_Hachama (Client)
```
#A14
auto eth0
iface eth0 inet static
    address 192.233.8.3
    netmask 255.255.248.0
    gateway 192.233.8.1
```

• Gamers (Gateway)
```
#A12
auto eth0
iface eth0 inet static
    address 192.233.10.130
    netmask 255.255.255.252
    gateway 192.233.10.129

#A13
auto eth1
iface eth1 inet static
    address 192.233.10.1
    netmask 255.255.255.128
```

• Korone (Client)
```
#A13
auto eth0
iface eth0 inet static
    address 192.233.10.2
    netmask 255.255.255.128
    gateway 192.233.10.1
```

• Okayu (Client)
```
#A13
auto eth0
iface eth0 inet static
    address 192.233.10.3
    netmask 255.255.255.128
    gateway 192.233.10.1
```

• Mio (Client)
```
#A13
auto eth0
iface eth0 inet static
    address 192.233.10.4
    netmask 255.255.255.128
    gateway 192.233.10.1
```


# Cisco Packet Tracker
Pada CPT ini kami menggunakan `VLSM`
## Topology CPT
![topologi mod4 IT33](https://github.com/user-attachments/assets/cd0b8356-f295-4c5f-a31f-2439f8c0bee1)

## Rute 
![Screenshot 2024-11-17 230749](https://github.com/user-attachments/assets/c9c42887-ef78-4a09-8f42-ef4c570c8759)

## Pembagian Area Subnet
![Screenshot 2024-11-17 230804](https://github.com/user-attachments/assets/4af5bfd0-b1df-49ca-a3c9-6e35f73f9cf1)

## Pembagian IP
![Screenshot 2024-11-17 231052](https://github.com/user-attachments/assets/717b0d9b-88ab-4e7b-b9a1-475c836d7bc6)

## Tree
![VLSM Tree drawio](https://github.com/user-attachments/assets/5057ab61-f244-4665-9dc8-199510f7706a)






