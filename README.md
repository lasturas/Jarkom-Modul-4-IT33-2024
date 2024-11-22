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
   - [Config GNS](#config-gns)
   - [Routing GNS](#routing-gns)
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

## Routing GNS

## Dokumentasi 
### irys --> mio 
![image](https://github.com/user-attachments/assets/226eb961-d128-4cde-b7ec-f726f53ef75e)

### mio --> irys 
![image](https://github.com/user-attachments/assets/2d4cbe5b-620f-4c32-8c08-25c7a8f6de3d)


### kroni --> zeta
![image](https://github.com/user-attachments/assets/056dfb2d-8a0c-42f4-9f7e-252a9794ac2c)

### zeta --> kroni 
![image](https://github.com/user-attachments/assets/f39125c1-f0fc-4846-8c8b-06377a075103)






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

## Konfigurasi IP

### Subnet A1

Hololive (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.73 255.255.255.252
no shutdown
```

Holo-ID (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.74 255.255.255.252
no shutdown
```

### Subnet A2

Holo-ID (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.93 255.255.255.252
no shutdown
```

AREA15 (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.94 255.255.255.252
no shutdown
```

### Subnet A3

AREA15 (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.8.1 255.255.252.0
no shutdown
```

Moona (Device)
```
Interface fa0
IP Address: 192.233.8.2
Subnet Mask: 255.255.252.0
Gateway: 192.233.8.1
```

Risu (Device)
```
Interface fa0
IP Address: 192.233.8.3
Subnet Mask: 255.255.252.0
Gateway: 192.233.8.1
```

lofi (Device)
```
Interface fa0
IP Address: 192.233.8.4
Subnet Mask: 255.255.252.0
Gateway: 192.233.8.1
```

### Subnet A4

Holo-ID (Router)
```
enable
configure terminal
interface fa1/0
ip address 192.233.19.97 255.255.255.252
no shutdown
```

holoro (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.98 255.255.255.252
no shutdown
```

### Subnet A5

holoro (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.18.193 255.255.255.192
no shutdown
```

Ollie (Device)
```
Interface fa0
IP Address: 192.233.18.194
Subnet Mask: 255.255.255.192
Gateway: 192.233.18.193
```

Anya (Device)
```
Interface fa0
IP Address: 192.233.18.195
Subnet Mask: 255.255.255.192
Gateway: 192.233.18.193
```

Reine (Device)
```
Interface fa0
IP Address: 192.233.18.196
Subnet Mask: 255.255.255.192
Gateway: 192.233.18.193
```

### Subnet A6

Holo-ID (Router)
```
enable
configure terminal
interface fa1/1
ip address 192.233.19.101 255.255.255.252
no shutdown
```

holoh3ro (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.102 255.255.255.252
no shutdown
```

### Subnet A7

holoh3ro (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.16.1 255.255.254.0
no shutdown
```

Zeta (Device)
```
Interface fa0
IP Address: 192.233.16.2
Subnet Mask: 255.255.254.0
Gateway: 192.233.16.1
```

Kaela (Device)
```
Interface fa0
IP Address: 192.233.16.3
Subnet Mask: 255.255.254.0
Gateway: 192.233.16.1
```

Kobo (Device)
```
Interface fa0
IP Address: 192.233.16.4
Subnet Mask: 255.255.254.0
Gateway: 192.233.16.1
```

### Subnet A8

Hololive (Router)
```
enable
configure terminal
interface fa1/1
ip address 192.233.19.105 255.255.255.252
no shutdown
```

HoloJP (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.106 255.255.255.252
no shutdown
```

### Subnet A9

Holo-JP (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.65 255.255.255.248
no shutdown
```

DEV_IS (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.66 255.255.255.248
no shutdown
```

GEN:0 (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.67 255.255.255.248
no shutdown
```

### Subnet A10

DEV_IS (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.33 255.255.255.240
no shutdown
```

Ririka_Rade (Device)
```
Interface fa0
IP Address: 192.233.19.34
Subnet Mask: 255.255.255.240
Gateway: 192.233.19.33
```

Ao (Device)
```
Interface fa0
IP Address: 192.233.19.35
Subnet Mask: 255.255.255.240
Gateway: 192.233.19.33
```

Hajime_Kanade (Device)
```
Interface fa0
IP Address: 192.233.19.36
Subnet Mask: 255.255.255.240
Gateway: 192.233.19.33
```

### Subnet A11

GEN:0 (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.0.1 255.255.248.0
no shutdown
```

GEN:1 (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.0.2 255.255.248.0
no shutdown
```

MiComet (Device)
```
Interface fa0
IP Address: 192.233.0.3
Subnet Mask: 255.255.248.0
Gateway: 192.233.0.1
```

Sora_Robo_AZK (Device)
```
Interface fa0
IP Address: 192.233.0.4
Subnet Mask: 255.255.248.0
Gateway: 192.233.0.1
```

### Subnet A12

GEN:1 (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.14.1 255.255.254.0
no shutdown
```

FBK_Matsuri (Device)
```
Interface fa0
IP Address: 192.233.14.2
Subnet Mask: 255.255.254.0
Gateway: 192.233.14.1
```

Aki_Hachama (Device)
```
Interface fa0
IP Address: 192.233.14.3
Subnet Mask: 255.255.254.0
Gateway: 192.233.14.1
```

### Subnet A13

GEN:1 (Router)
```
enable
configure terminal
interface fa1/0
ip address 192.233.19.77 255.255.255.252
no shutdown
```

GAMERS (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.78 255.255.255.252
no shutdown
```

### Subnet A14

GAMERS (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.18.1 255.255.255.128
no shutdown
```

Korone (Device)
```
Interface fa0
IP Address: 192.233.18.2
Subnet Mask: 255.255.255.128
Gateway: 192.233.18.1
```

Okayu (Device)
```
Interface fa0
IP Address: 192.233.18.3
Subnet Mask: 255.255.255.128
Gateway: 192.233.18.1
```

Mio (Device)
```
Interface fa0
IP Address: 192.233.18.4
Subnet Mask: 255.255.255.128
Gateway: 192.233.18.1
```

### Subnet A15

Hololive (Router)
```
enable
configure terminal
interface fa1/0
ip address 192.233.19.81 255.255.255.252
no shutdown
```

HoloEN (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.82 255.255.255.252
no shutdown
```

### Subnet A16

HoloEN (Router)
```
enable
configure terminal
interface fa1/0
ip address 192.233.19.85 255.255.255.252
no shutdown
```

HoloAdvent (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.86 255.255.255.252
no shutdown
```

### Subnet A17

HoloAdvent (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.1 255.255.255.224
no shutdown
```

FuwaMoco (Device)
```
Interface fa0
IP Address: 192.233.19.2
Subnet Mask: 255.255.224.0
Gateway: 192.233.19.1
```

Shiori_Nerissa (Device)
```
Interface fa0
IP Address: 192.233.19.3
Subnet Mask: 255.255.224.0
Gateway: 192.233.19.1
```

Biboo (Device)
```
Interface fa0
IP Address: 192.233.19.4
Subnet Mask: 255.255.224.0
Gateway: 192.233.19.1
```

### Subnet A18

HoloEN (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.89 255.255.255.252
no shutdown
```

Holo-Myth (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.90 255.255.255.252
no shutdown
```

### Subnet A19

Holo-Myth (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.12.1 255.255.254.0
no shutdown
```

Gura_Ame_Ina (Device)
```
Interface fa0
IP Address: 192.233.12.2
Subnet Mask: 255.255.254.0
Gateway: 192.233.12.1
```

Kiara_Calli (Device)
```
Interface fa0
IP Address: 192.233.12.3
Subnet Mask: 255.255.254.0
Gateway: 192.233.12.1
```

### Subnet A20

Holo-Myth (Router)
```
enable
configure terminal
interface fa1/0
ip address 192.233.19.49 255.255.255.248
no shutdown
```

Project-Hope (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.50 255.255.255.248
no shutdown
```

Holo-Council (Router)
```
enable
configure terminal
interface fa0/0
ip address 192.233.19.51 255.255.255.248
no shutdown
```

### Subnet A21

Project-Hope (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.19.57 255.255.255.248
no shutdown
```

Irys (Device)
```
Interface fa0
IP Address: 192.233.19.58
Subnet Mask: 255.255.255.248
Gateway: 192.233.19.57
```

### Subnet A22

Holo-Council (Router)
```
enable
configure terminal
interface fa0/1
ip address 192.233.18.129 255.255.255.192
no shutdown
```

Kronii_Mumei (Device)
```
Interface fa0
IP Address: 192.233.18.130
Subnet Mask: 255.255.255.192
Gateway: 192.233.18.129
```

Bae_Fauna (Device)
```
Interface fa0
IP Address: 192.233.18.131
Subnet Mask: 255.255.255.192
Gateway: 192.233.18.129
```
## Konfigurasi Routing

### Sisi Kanan (Holo-ID)

Hololive
```
enable
configure terminal
ip route 192.233.19.92 255.255.255.252 192.233.19.74
ip route 192.233.8.0 255.255.252.0 192.233.19.74
ip route 192.233.19.96 255.255.255.252 192.233.19.74
ip route 192.233.18.192 255.255.255.192 192.233.19.74
ip route 192.233.19.100 255.255.255.252 192.233.19.74
ip route 192.233.16.0 255.255.254.0 192.233.19.74
do write
```

Holo-ID
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.73
ip route 192.233.8.0 255.255.252.0 192.233.19.94
ip route 192.233.18.192 255.255.255.192 192.233.19.98
ip route 192.233.16.0 255.255.254.0 192.233.19.102
do write
```

AREA15
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.93
do write
```

holoro
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.97
do write
```

holoh3ro
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.101
do write
```

### Sisi Bawah (HoloJP)

Hololive
```
enable
configure terminal
ip route 192.233.19.64 255.255.255.248 192.233.19.106
ip route 192.233.19.32 255.255.255.240 192.233.19.106
ip route 192.233.0.0 255.255.248.0 192.233.19.106
ip route 192.233.14.0 255.255.254.0 192.233.19.106
ip route 192.233.19.76 255.255.255.252 192.233.19.106
ip route 192.233.18.0 255.255.255.128 192.233.19.106
do write
```

Holo-JP
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.105
ip route 192.233.19.32 255.255.255.240 192.233.19.66
ip route 192.233.0.0 255.255.248.0 192.233.19.67
ip route 192.233.14.0 255.255.254.0 192.233.19.67
ip route 192.233.19.76 255.255.255.252 192.233.19.67
ip route 192.233.18.0 255.255.255.128 192.233.19.67
do write
```

DEV_IS
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.65
ip route 192.233.0.0 255.255.248.0 192.233.19.67
ip route 192.233.14.0 255.255.254.0 192.233.19.67
ip route 192.233.19.76 255.255.255.252 192.233.19.67
ip route 192.233.18.0 255.255.255.128 192.233.19.67
do write
```

GEN:0
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.65
ip route 192.233.19.32 255.255.255.240 192.233.19.66
ip route 192.233.14.0 255.255.254.0 192.233.0.2
ip route 192.233.19.76 255.255.255.252 192.233.0.2
ip route 192.233.18.0 255.255.255.128 192.233.0.2
do write
```

GEN:1
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.0.1
ip route 192.233.18.0 255.255.255.128 192.233.19.78
do write
```

GAMERS
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.77
do write
```

### Sisi Kiri (HoloEN)

Hololive
```
enable
configure terminal
ip route 192.233.19.84 255.255.255.252 192.233.19.82
ip route 192.233.19.0 255.255.255.224 192.233.19.82
ip route 192.233.19.88 255.255.255.252 192.233.19.82
ip route 192.233.12.0 255.255.254.0 192.233.19.82
ip route 192.233.19.48 255.255.255.248 192.233.19.82
ip route 192.233.19.56 255.255.255.248 192.233.19.82
ip route 192.233.18.128 255.255.255.192 192.233.19.82
do write
```

HoloEN
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.81
ip route 192.233.19.0 255.255.255.224 192.233.19.86
ip route 192.233.12.0 255.255.254.0 192.233.19.90
ip route 192.233.19.48 255.255.255.248 192.233.19.90
ip route 192.233.19.56 255.255.255.248 192.233.19.90
ip route 192.233.18.128 255.255.255.192 192.233.19.90
do write
```

HoloAdvent
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.85
do write
```

Holo-Myth
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.89
ip route 192.233.19.56 255.255.255.248 192.233.19.50
ip route 192.233.18.128 255.255.255.192 192.233.19.51
do write
```

Project-Hope
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.49
ip route 192.233.18.128 255.255.255.192 192.233.19.51
do write
```

Holo-Council
```
enable
configure terminal
ip route 0.0.0.0 0.0.0.0 192.233.19.49
ip route 192.233.19.56 255.255.255.248 192.233.19.50
do write
```





