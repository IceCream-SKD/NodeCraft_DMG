# NodeCraft

แอป desktop บน macOS สำหรับวิศวกร network — รองรับทั้ง Apple Silicon และ Intel (universal)

## ดาวน์โหลด

ไปที่หน้า [Releases](../../releases/latest) แล้วโหลดไฟล์ `NodeCraft-<version>-universal.dmg`

## ติดตั้ง

1. เปิดไฟล์ `.dmg` แล้วลาก **NodeCraft** ไปไว้ในโฟลเดอร์ **Applications**
2. เปิดแอปครั้งแรก macOS จะเตือนว่าเปิดไม่ได้ เพราะแอป ad-hoc signed (ไม่มี Apple Developer ID)
3. ไปที่ **System Settings → Privacy & Security** เลื่อนลงไปกด **Open Anyway** แล้วยืนยันอีกครั้ง

ครั้งต่อไปเปิดได้ตามปกติ

## ทำอะไรได้บ้าง

| กลุ่ม | หน้า | ทำอะไร |
|---|---|---|
| Overview | Dashboard | ภาพรวมสถานะโฮสต์และ latency (แสดงเฉพาะค่าที่วัดได้จริง) |
| | Monitoring | ping โฮสต์ต่อเนื่องแบบตาราง NOC แยก profile มีกราฟ latency และ ping log |
| Configuration | Config Backup | ดึง config อุปกรณ์ Cisco ผ่าน SSH / Telnet / serial console เก็บ credential แบบเข้ารหัส |
| | Config Compare | เทียบ config สองไฟล์แบบ side-by-side |
| Documentation | Topology | สร้างแผนผัง network จากไฟล์ backup (CDP/LLDP) export เป็น PNG / draw.io / Excel |
| | Port Mapping | สร้างไฟล์ Excel Port Mapping จาก config IOS / NX-OS / ASA / WLC |
| Tools | Traceroute, Port Scanner, IP Calculator | traceroute, สแกน TCP port, คำนวณ subnet IPv4/IPv6 |

## ข้อมูลของผู้ใช้

ข้อมูลทั้งหมดเก็บในเครื่องที่ `~/Library/Application Support/NodeCraft/` — ถอนการติดตั้งแอปไม่ลบข้อมูลนี้

> repo นี้มีไว้แจกไฟล์ติดตั้งเท่านั้น
