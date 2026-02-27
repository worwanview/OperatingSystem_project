# Operating System & Distributed System Project

โปรเจกต์นี้เป็นงานสำหรับรายวิชา **Operating System / Distributed Systems**  
พัฒนาโดยใช้ภาษา **Java** เพื่อศึกษาการทำงานของระบบปฏิบัติการและระบบกระจาย

---

## เนื้อหาของโปรเจกต์

### 1. File Transfer System
- เปรียบเทียบการส่งไฟล์แบบ **Copy I/O** และ **Zero-Copy**
- ใช้ Socket และ Java NIO
- วัดเวลาและประสิทธิภาพในการรับ–ส่งไฟล์

ไฟล์หลัก:
- `Server.java`
- `Client.java`

---

### 2. Distributed Process System
- จำลองระบบ process แบบกระจาย
- มีการส่ง **Heartbeat** เพื่อตรวจจับ process ล่ม
- ใช้ **Leader Election (Ring Algorithm)** เพื่อเลือก Boss ใหม่เมื่อ Leader ล่ม
- รองรับการทำงานแบบหลาย thread

ไฟล์หลัก:
- `ProcessNode.java`

---

## แนวคิดที่เกี่ยวข้อง
- Process และ PID
- Inter-Process Communication (Socket)
- Multithreading
- Failure Detection
- Leader Election

---

## วิธีใช้งานโดยสรุป
- รัน `Server.java` และ `Client.java` เพื่อทดสอบการส่งไฟล์
- รัน `ProcessNode.java` หลาย instance เพื่อจำลองระบบ Distributed

