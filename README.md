# GEE + Vibe Coding for Forestry

คอร์ส **Google Earth Engine สำหรับงานป่าไม้** 3 วัน วันละ 2 ชั่วโมง สอนผ่านการ "สั่งงาน AI" (vibe coding) — คุณอธิบายสิ่งที่ต้องการเป็นภาษาอังกฤษ ให้ AI เขียนโค้ดให้ แล้วรันจริงใน Google Colab

ไม่ต้องมีพื้นฐานเขียนโปรแกรมหรือ GIS มาก่อน ทักษะที่แท้จริงของคอร์สนี้คือ**การตรวจสอบว่าคำตอบของ AI ถูกต้องหรือไม่** ไม่ใช่การเขียนโค้ดเอง

---

## เริ่มต้นก่อนวันที่ 1 (ทำล่วงหน้าอย่างน้อย 3 วัน)

1. อ่าน **[คู่มือตั้งค่า Day 0](00-setup/Day0-Setup-Guide.pdf)** — สมัคร Google Earth Engine ด้วย Gmail ส่วนตัว และติดตั้ง **Antigravity** (AI ผู้ช่วยฟรีที่ใช้ตลอดคอร์ส)
2. รัน **[00_check_gee_access.ipynb](00-setup/00_check_gee_access.ipynb)** ใน Google Colab เพื่อยืนยันว่าบัญชีของคุณใช้งานได้จริง — ต้องเห็นคำว่า **ALL CHECKS PASSED**
3. จดจังหวัดที่คุณสนใจไว้ล่วงหน้า — ทุก lab ให้คุณเปลี่ยนพื้นที่ศึกษาเป็นจังหวัดของตัวเองได้

ถ้าติดปัญหาระหว่างตั้งค่า เปิด **[คู่มือแก้ปัญหา](05-handouts/Troubleshooting.pdf)** ไว้ข้างๆ — ครอบคลุม error ที่พบได้บ่อยที่สุด

---

## ตารางเรียน 3 วัน

ดูเวลาโดยละเอียดได้ที่ **[ตารางการสอน (ไทย)](05-handouts/Course-Schedule-th.pdf)** หรือ **[English](05-handouts/Course-Schedule.pdf)**

| วัน | หัวข้อ | สไลด์ | แบบฝึกหัด | Lab (Colab) |
|---|---|---|---|---|
| **1** | พื้นฐาน RS, Earth Engine, Vibe coding | [TH](01-slides/day1-th.pdf) · [EN](01-slides/day1.pdf) | [พิมพ์](03-exercises/Exercise-Day1.pdf) · [กรอกในเครื่อง](03-exercises/Exercise-Day1-fillable.pdf) | [Lab 1](02-notebooks/student/lab1_first_map.ipynb) · [Lab 2](02-notebooks/student/lab2_landcover.ipynb) |
| **2** | จำแนกประเภทป่า, คาร์บอน | [TH](01-slides/day2-th.pdf) · [EN](01-slides/day2.pdf) | [พิมพ์](03-exercises/Exercise-Day2.pdf) · [กรอกในเครื่อง](03-exercises/Exercise-Day2-fillable.pdf) | [Lab 3](02-notebooks/student/lab3_forest_type_rf.ipynb) · [Lab 4](02-notebooks/student/lab4_carbon.ipynb) |
| **3** | ไฟป่า, ภูมิอากาศ, โครงงานย่อย | [TH](01-slides/day3-th.pdf) · [EN](01-slides/day3.pdf) | [พิมพ์](03-exercises/Exercise-Day3.pdf) · [กรอกในเครื่อง](03-exercises/Exercise-Day3-fillable.pdf) | [Lab 5](02-notebooks/student/lab5_fire.ipynb) · [Lab 6](02-notebooks/student/lab6_climate.ipynb) · [โครงงาน](02-notebooks/student/miniproject_template.ipynb) |

**สไลด์:** เลือกภาษาไทยหรืออังกฤษก็ได้ เนื้อหาเหมือนกัน ต่างแค่ภาษา (ศัพท์เทคนิค ชื่อชุดข้อมูล และโค้ดยังคงเป็นอังกฤษในทั้งสองเวอร์ชัน เพราะเอกสารจริงของ Earth Engine เป็นอังกฤษ)

**แบบฝึกหัด:** มีสองแบบให้เลือกเนื้อหาเดียวกัน — **"พิมพ์"** สำหรับปริ้นแล้วเขียนด้วยมือ, **"กรอกในเครื่อง"** เปิดด้วยโปรแกรมอ่าน PDF (Adobe Acrobat, Preview บน Mac ฯลฯ) แล้วพิมพ์ตอบได้เลยโดยไม่ต้องปริ้น

---

## เอกสารอ้างอิง (เก็บไว้ใช้ตลอดคอร์ส)

- **[AI Prompt Cookbook](05-handouts/AI-Prompt-Cookbook.pdf)** — สูตร PROMPT และตัวอย่าง prompt ที่ใช้ได้จริง เก็บไว้ใช้ต่อหลังจบคอร์สได้เลย
- **[GEE Dataset Cheat Sheet](05-handouts/GEE-Dataset-Cheatsheet.pdf)** — รายชื่อชุดข้อมูล Earth Engine ที่ตรวจสอบแล้วว่าใช้งานได้จริง พร้อมหน่วยและข้อควรระวัง
- **[Glossary EN-TH](05-handouts/Glossary-EN-TH.pdf)** — ศัพท์เทคนิค ~70 คำ พร้อมคำแปลไทย
- **[Troubleshooting](05-handouts/Troubleshooting.pdf)** — error ที่พบบ่อยที่สุดในคอร์สนี้ พร้อมวิธีแก้

---

## AI ที่ใช้ในคอร์สนี้: Antigravity

Antigravity คือ AI ผู้ช่วยฟรีของ Google ที่คุณจะสั่งงานตลอดคอร์ส — แต่มีกฎสำคัญข้อเดียว:

> **Antigravity เขียนโค้ด · Colab เป็นคนรันโค้ด**

Antigravity เปิดและรันไฟล์ได้เองด้วย แต่ในคอร์สนี้ **ใช้แค่ช่องแชทของมันเท่านั้น** — พิมพ์ prompt ขอโค้ด รับโค้ดกลับมา แล้ว**คัดลอกไปวางรันใน Colab** เอง ทุก lab และทุกแผนที่ที่คุณจะเห็นถูกออกแบบมาให้แสดงผลใน Colab เท่านั้น

ถ้า Antigravity ใช้ไม่ได้ชั่วคราว (โควตาเต็มรายสัปดาห์) สลับไปใช้ **Gemini ที่มีอยู่ในตัว Colab อยู่แล้ว** ได้ทันที ไม่ต้องสมัครบัญชีเพิ่ม

---

## ก่อนมาเรียน ต้องมีอะไรบ้าง

- โน้ตบุ๊กที่ติดตั้งโปรแกรมเองได้ (ไม่ใช่เครื่องที่ล็อกไว้หรือใช้ร่วมกับคนอื่น)
- บัญชี Gmail ส่วนตัว (ไม่ใช่บัญชีของมหาวิทยาลัย — มักถูกบล็อกไม่ให้ใช้ API ภายนอก)
- Antigravity ติดตั้งและล็อกอินแล้ว (ดูขั้นตอนใน [คู่มือตั้งค่า Day 0](00-setup/Day0-Setup-Guide.pdf))
- ไม่ต้องมีบัตรเครดิต — ทุกอย่างในคอร์สนี้ฟรี
