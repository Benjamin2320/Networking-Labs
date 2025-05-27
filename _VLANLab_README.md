# Networking-Labs

# VLAN Configuration and Trunking

## Overview
This lab demonstrates the configuration of VLANs, trunking, native VLANs, and testing connectivity using Cisco Packet Tracer.
VLANs are useful because they let you split a network into smaller, virtual sections that act like subnets. This way, devices can communicate with each other as if they were on the same network, even if they’re physically spread out. It helps control layer 2 traffic and improves both security and efficiency.

## Objectives
- Create VLANs and assign switch ports
- Configure trunk ports
- Set native VLANs
- Limit VLANs on trunk links
- Test network connectivity

## Topology
![Screenshot 2025-05-26 170401](https://github.com/user-attachments/assets/7c727770-8035-4877-90bf-b0582d90ed31)

## 🧩 VLAN Creation and Naming

### Commands
```bash
vlan 10
name Operations
vlan 20
name Parking_Lot
vlan 99
name Management
vlan 1000
name Native
```

## VLAN Creation
![VLAN Setup]![Screenshot 2025-05-26 161933](https://github.com/user-attachments/assets/e8fbff94-b8d8-4de0-9314-16f6e1e8d4e3)

## 🔌 Port Assignment

📸 ![Assigned Ports to VLAN 99]![Screenshot 2025-05-26 164906](https://github.com/user-attachments/assets/42745989-3183-4cdc-b31c-33d49bd69f23)
  
> Assigned range of ports to VLAN 99 on SW1.

📸 ![Assigned VLAN to Single Port]![Screenshot 2025-05-26 163121](https://github.com/user-attachments/assets/d53a2155-a7e8-4999-9b78-ff50d89edab4)
  
> Assigned Fa0/6 to VLAN 10.
>
> ## 🌐 Management IP Configuration

📸 ![Set Management IP]![Screenshot 2025-05-26 162644](https://github.com/user-attachments/assets/bcb9322f-5a0b-43f0-bc48-4620f44b60ac)
  
> IP address applied to VLAN 99 for switch management.

---

## 🧪 Show Commands & Verification

📸 ![Final VLAN Table SW1]![Screenshot 2025-05-26 162634](https://github.com/user-attachments/assets/e8122724-8df3-4cf9-8cae-666bf214f717)
  
📸 ![Final VLAN Table SW2]![Screenshot 2025-05-26 163202](https://github.com/user-attachments/assets/b5eae672-7c41-4f4d-b058-67327c2292b1)
  
> Confirmed VLANs and interface assignments.

---

## 🌉 Trunking Verification

📸 ![Trunking on SW2]![Screenshot 2025-05-26 170438](https://github.com/user-attachments/assets/dc65dc2c-08aa-4eb1-a7c5-35a0b53bddde)
 
📸 ![Trunking on SW1]![Screenshot 2025-05-26 170425](https://github.com/user-attachments/assets/fa42e821-b781-420d-9589-f3da52362c89)
  
> Verified trunk port (Fa0/1) status and encapsulation on both switches.

---

## 🧪 Ping Test

📸 ![Ping Result]![Screenshot 2025-05-26 161933](https://github.com/user-attachments/assets/ed023e4a-404d-4ea0-8a20-23a2ad30ede7)
  
> Successful ping confirms proper VLAN and trunk configuration.


## ✅ Conclusion
This lab demonstrated:
- Creating and managing VLANs
- Assigning access ports
- Setting a trunk between switches
- Verifying with ping and show commands

## Folder Structure
---Networking-Labs/

├── README.md

├── VLAN-Lab/

│   ├── README.md

│   └── screenshots/

│       ├── Screenshot 2025-05-26 165855.png

│       ├── Screenshot 2025-05-26 165254.png

│       ├── Screenshot 2025-05-26 164906.png

│       ├── Screenshot 2025-05-26 163121.png

│       ├── Screenshot 2025-05-26 162644.png

│       ├── Screenshot 2025-05-26 162634.png

│       ├── Screenshot 2025-05-26 163202.png

│       ├── Screenshot 2025-05-26 170438.png

│       ├── Screenshot 2025-05-26 170425.png

│       ├── Screenshot 2025-05-26 161933.png

│       └── Screenshot 2025-05-26 161953.png

