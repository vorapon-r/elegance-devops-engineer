# แบบทดสอบตำแหน่ง DevOps Engineer  

ยินดีต้อนรับสู่แบบทดสอบสำหรับตำแหน่ง **DevOps Engineer**!  
โปรดทำตามคำแนะนำในส่วนต่าง ๆ ด้านล่างนี้ และส่งคำตอบหรือโค้ดทั้งหมดผ่านลิงก์ Repository หรือไฟล์ ZIP  

---

## **ส่วนที่ 1: การเขียน Script**  
### ภารกิจ  
เขียน Script โดยใช้ **Python** หรือ **Bash** ที่สามารถทำสิ่งต่อไปนี้:  
1. สร้าง Docker Image สำหรับแอปพลิเคชัน **Python Flask** แบบง่าย  
2. ตั้ง Tag ให้กับ Image โดยใช้หมายเลขเวอร์ชันที่ส่งมาเป็น Argument  
3. Push Docker Image ไปยัง Docker Registry  
4. Deploy Image ไปยัง Kubernetes Cluster โดยใช้คำสั่ง `kubectl`  

### เพิ่มคะแนน (Bonus)  
- เพิ่ม Readiness และ Liveness Probe ใน Kubernetes Deployment  

---

## **ส่วนที่ 2: การตั้งค่า CI/CD Pipeline**  
### ภารกิจ  
สร้างไฟล์การตั้งค่า **YAML** สำหรับเครื่องมือ CI/CD เช่น **GitLab CI/CD** โดยต้องทำสิ่งต่อไปนี้:  
1. รัน Automated Tests  
2. Build และ Push Docker Image ไปยัง Container Registry  
3. Deploy แอปพลิเคชันไปยัง Kubernetes Cluster  

### เพิ่มคะแนน (Bonus)  
- เพิ่มขั้นตอนการแจ้งเตือนใน **Slack Channel** เมื่อการ Deploy สำเร็จ  

---

## **ส่วนที่ 3: การแก้ปัญหาและการ Monitoring**  
### สถานการณ์  
ใน **Production Kubernetes Cluster** ทีมพบว่า API มีการตอบสนองที่ช้าลง ซึ่งอาจเกิดจากปัญหาต่อไปนี้:  
- การใช้ CPU หรือ Memory ใน Pod สูงเกินไป  
- มี Error ใน API Logs  
- Latency ของเครือข่ายสูง  

### ภารกิจ  
1. เขียนแผนตรวจสอบเพื่อระบุสาเหตุ โดยใช้เครื่องมือเช่น **Prometheus**, **Grafana** หรือ **ELK Stack**  
2. เสนอวิธีแก้ปัญหา  
3. แนะนำแนวทางป้องกันปัญหาลักษณะนี้ในอนาคต  

---

## **ส่วนที่ 4: คำถามเชิงแนวคิด**  
โปรดตอบคำถามต่อไปนี้:  
1. **Service Mesh และ API Gateway**  
   - อธิบายความแตกต่างระหว่าง **Istio** และ **Kong**  
   - ยกตัวอย่างการใช้งานทั้งสองร่วมกัน  

2. **Security และ Compliance**  
   - คุณจะป้องกันความปลอดภัยใน CI/CD Pipeline ได้อย่างไร?  
   - คุณจะจัดการ Kubernetes Secrets อย่างปลอดภัยได้อย่างไร?  

3. **Cloud และการขยายระบบ (Scaling)**  
   - คุณจะออกแบบ Kubernetes Cluster บน **AWS** ให้รองรับ High Availability ได้อย่างไร?  
   - อธิบายข้อดีของการใช้ **Horizontal Pod Autoscaling** ใน Kubernetes  

---

## **ส่วนที่ 5: ภารกิจ Hands-on (ตัวเลือกเสริม)**  
### ภารกิจ  
1. ตั้งค่า CI/CD Pipeline แบบสมบูรณ์ โดยใช้ **GitLab**, **CircleCI** เพื่อ:  
   - รัน Test อย่างง่าย  
   - Build Docker Image  
   - Deploy ไปยัง Kubernetes Cluster  

2. ใช้ **Kubernetes** เพื่อ Deploy แอปพลิเคชัน (Flask หรือ Node.js) พร้อมกับ:  
   - ตั้งค่า **Istio** สำหรับ Service Mesh  
   - ตั้งค่า **Kong** เป็น API Gateway  

### สิ่งที่ต้องส่ง  
- ลิงก์ Repository ที่มีไฟล์การตั้งค่าทั้งหมด (รวมถึงไฟล์ CI/CD, Kubernetes Configs และ Script)  
- หรือไฟล์ ZIP พร้อมคำแนะนำการใช้งาน  

---

## การประเมิน  
### คะแนนเต็ม: 100 คะแนน  
- **ส่วนที่ 1: การเขียน Script (20 คะแนน)**: คุณภาพโค้ด, ประสิทธิภาพ, และความครบถ้วน  
- **ส่วนที่ 2: การตั้งค่า CI/CD Pipeline (20 คะแนน)**: ความชัดเจนและการทำงานได้จริง  
- **ส่วนที่ 3: การแก้ปัญหา (20 คะแนน)**: ความลึกซึ้งของการวิเคราะห์และแนวทางแก้ไข  
- **ส่วนที่ 4: คำถามเชิงแนวคิด (20 คะแนน)**: การอธิบายความเข้าใจที่ดี  
- **ส่วนที่ 5: ภารกิจ Hands-on (20 คะแนน)**: ความครบถ้วนและความถูกต้องของงาน  

---

## หมายเหตุ  
- โปรดเขียนคำตอบหรือโค้ดให้มีคำอธิบายที่ชัดเจน  
- คุณสามารถเลือกเครื่องมือหรือเทคโนโลยีที่คุณถนัดได้ (เช่น Docker, Kubernetes, CI/CD Tools)  
- แบบทดสอบนี้ออกแบบมาเพื่อประเมินทักษะและแนวคิดของคุณในโลกจริง  

ขอให้โชคดี!  
**Awesome !!!**
