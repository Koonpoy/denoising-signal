# Denoising-Signal

โปรแกรม Denoising-Signal เป็นโปรแกรมสำหรับลดสัญญาณรบกวนโดยใช้ Fast Fourier Transform (FFT) ในการแปลง และฟังก์ชัน ที่สามารถฟังเสียงต้นฉบับและเสียงที่ถูก Denoising แล้วได้ และสามารถดาวน์โหลดไฟล์ที่ถูกแปลงแล้วนำไปใช้งานต่อได้

![image](https://user-images.githubusercontent.com/85865681/202138982-0cad4296-364b-4757-ac65-efa61f0eca09.png)

# สัญญาณเสียง 4 แบบ

![image](https://user-images.githubusercontent.com/85865681/202140578-f33b188c-ca31-447a-9c01-c31d3f5f7f64.png)

ช่องแรกคือ สัญญาณเสียงต้นฉบับ 
![image](https://user-images.githubusercontent.com/85865681/202144610-a9c1c886-dc4a-4aa8-8ad3-ee2a55ac950c.png)

ช่องสองคือ สัญญาณเสียงหลังจากผ่าน Fast Fourier Transform
![image](https://user-images.githubusercontent.com/85865681/202144630-ebb3d451-a95e-447a-b3e0-9d2aa6f0d475.png)

ช่องสามคือ สัญญาณเสียง Power spectrum of Audio
![image](https://user-images.githubusercontent.com/85865681/202144640-d48d93f3-f18e-474d-b10e-32ef917f7669.png)

ช่องสุดท้ายทางขวามือคือ สัญญาณเสียงที่ถูก Denoising เสร็จเรียบร้อยแล้ว
![image](https://user-images.githubusercontent.com/85865681/202144682-0b3528af-6492-466e-a340-bf7cc10e59ae.png)

# Set Denoise Vaule

สามารถ set ค่า PSD เพื่อเลือกระดับในการตัดสัญญาณรบกวนของสัญญาณเสียงได้
![image](https://user-images.githubusercontent.com/85865681/202145751-37766111-5f9a-48c1-8d88-b497b3f39760.png)

# Function ClearAll Import Export

ในตอนแรกตัวโปรแกรมจะสามารถกดได้แค่ปุ่มเดียวคือปุ่ม Import คือการนำไฟล์ Audio ที่ต้องการ Denoise เข้ามาแปลง
![image](https://user-images.githubusercontent.com/85865681/202139352-04fe756a-2267-45f7-9cd1-261e33540691.png)

เมื่อ Import จะมีสัญญาณโชว์ทั้งหมด 4 แบบและสามารถกดปุ่มที่เหลือได้ ปุ่ม ClearAll เมื่อกดแล้วจะล้างไฟล์ที่ถูก Import เข้ามา ปุ่ม Export เมื่อกดแล้วจะทำการ Download ไฟล์ที่ถูกแปลงด้วย FFT แล้ว
<p float="left">
  <img src="https://user-images.githubusercontent.com/85865681/202139504-e132601d-a2a0-453d-81da-e0004570c7bb.png" width="50%"/>
  <img src="https://user-images.githubusercontent.com/85865681/202140578-f33b188c-ca31-447a-9c01-c31d3f5f7f64.png" width="50%"/>
</p>

# Future Play Pause Stop Volume
เมื่องทำการ Import ไฟล์ Audio เข้ามาแล้วจะสามารถใช้งานฟีเจอร์นี้ได้ โดยการ Play เพิ่มเริ่ม กด Pause เพิ่อหยุดชั่วคราวและกดปุ่มเดิมเพื่อเล่นต่อ กด Stop เพื่อหยุดการเล่นเสียงนั้น 
![image](https://user-images.githubusercontent.com/85865681/202147564-fd6ff7c0-f80b-44bc-a005-376dec2ef6a1.png)
![image](https://user-images.githubusercontent.com/85865681/202147612-778ac6d8-c1ce-4032-a59c-e7e7336bac65.png)
และสามารถปรับ Volume เพื่อเพิ่ม/ลดความดังของเสียงได้
![image](https://user-images.githubusercontent.com/85865681/202147653-0b2c26e5-3641-4eb6-acd3-76f7b00ef7a5.png)
