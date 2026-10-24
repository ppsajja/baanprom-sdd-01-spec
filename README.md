# baanprom-sdd-01-spec

repo ตัวอย่างของรายวิชา 517511-266 Requirement Engineering (AI-Native RE)
ภาควิชาคอมพิวเตอร์ คณะวิทยาศาสตร์ มหาวิทยาลัยศิลปากร

เคส: บ้านพร้อม (แพลตฟอร์มจองช่างซ่อมบ้าน)
ข้อมูลทั้งหมดในเคสนี้เป็นข้อมูลสมมติเพื่อการสอน

## repo นี้คืออะไร

repo นี้รวมชิ้นงานของกลุ่มตัวอย่าง (กลุ่ม X) จากบทเรียน 1 ถึง 7 เป็นไฟล์ Markdown ที่เปิดอ่านได้บน GitHub
ทุกไฟล์อยู่ใน docs/srs/ และเป็นต้นฉบับ (source of truth) ของเรื่องนั้น

สภาพของ repo คือ "ก่อนประกาศ Baseline B1"
ยังไม่มี spec.md, plan.md, tasks.md และยังไม่มีโค้ด
ทุกไฟล์ที่จะเข้า B1 ยังเขียนว่า "เสนอเข้า Baseline B1"

## ใช้เริ่มบทเรียนไหน และเป็นเฉลยของบทไหน

- ใช้เริ่มบทเรียน **Modern Specification และ SDD**
- เป็นเฉลยของบทเรียน 1 ถึง 7 คือ Modern RE, Problem Framing, Elicitation, Taxonomy, Stories Scenarios และ Use Cases, Prioritization และ Integrated Requirements Modelling

## ชุด repo ทั้ง 8

แต่ละ repo คือจุดเริ่มของบทหนึ่ง และเป็นเฉลยของบทก่อนหน้า repo ถัดไปจึงเป็นเฉลยของงานในบทนี้

| repo | ใช้เริ่มบท | ข้างในคือเฉลยของ |
|---|---|---|
| **baanprom-sdd-01-spec** (repo นี้) | Modern Specification และ SDD | ชิ้นงานบท 1 ถึง 7 (Problem Framing ถึง Integrated Modelling) |
| [baanprom-sdd-02-build](https://github.com/ppsajja/baanprom-sdd-02-build) | AI Build from Spec | Modern Specification และ SDD: spec plan tasks ที่กลุ่มเขียนเอง และ Baseline B1 |
| [baanprom-sdd-03-vv](https://github.com/ppsajja/baanprom-sdd-03-vv) | Verification, Validation และ Change | AI Build from Spec: โค้ดและ test ที่ AI สร้าง ac-results gaps CR-01 CR-02 |
| [baanprom-sdd-04-ops](https://github.com/ppsajja/baanprom-sdd-04-ops) | Operational, Security และ Privacy | V&V และ Change: RTM mockup CR-03 ถึง CR-06 Baseline B2 และ R1 ครบ (003 004) |
| [baanprom-sdd-05-ai](https://github.com/ppsajja/baanprom-sdd-05-ai) | Data, AI และ Agent | Operational, Security และ Privacy: CR-07 อนุมัติ และ Baseline B3 |
| [baanprom-sdd-06-accept](https://github.com/ppsajja/baanprom-sdd-06-accept) | RE in One Line และการตรวจรับ | Data, AI และ Agent: ผู้ช่วย AI UC-14 (CR-09) และ Baseline B4 |
| [baanprom-sdd-07-r1-done](https://github.com/ppsajja/baanprom-sdd-07-r1-done) | บทเสริม การตรวจรับและการส่งมอบ | RE in One Line และการตรวจรับ: ตรวจรับ R1 (CR-10) และ Baseline B5 |
| [baanprom-sdd-08-complete](https://github.com/ppsajja/baanprom-sdd-08-complete) | (ระบบสมบูรณ์ของวิชา) | บทเสริม การตรวจรับและการส่งมอบ: R2 ครบทุก UC ส่งมอบตาม TOR และ Baseline B7 |

## อะไรใหม่เมื่อเทียบกับ repo ก่อนหน้า

repo นี้เป็นตัวแรกของชุด ไม่มี repo ก่อนหน้า
ตารางนี้บอกว่าแต่ละไฟล์คือชิ้นงานของบทไหน

| ไฟล์ | สิ่งที่มี | เพราะอะไร |
|---|---|---|
| docs/srs/problem-statement.md | เคส ห้าชั้น Canvas 7 ช่อง PB-01 ถึง PB-04 5 Whys Goal Model ขอบเขต JTBD Journey As-Is | ชิ้นงานบท Modern RE และ Problem Framing |
| docs/srs/stakeholders.md | SH-01 ถึง SH-06 เช็กลิสต์ 13 บทบาท Power-Interest Grid | ชิ้นงานบท Problem Framing |
| docs/srs/evidence.md | แผนเก็บความต้องการ EV-001 ถึง EV-035 (เท่าที่หน้าบทเรียนแสดง) ความขัดแย้ง ร่าง REQ ชุดแรก | ชิ้นงานบท Elicitation |
| docs/srs/catalogue.md | REQ ทุกข้อที่หน้าบทเรียนแสดง พร้อมหมวด MoSCoW สถานะ ที่มา | ชิ้นงานบท Taxonomy ปรับปรุงถึงบท Modelling |
| docs/srs/decisions.md | MoSCoW Kano weighted scoring จุดพลิก แผนรุ่น DR-01 DR-02 | ชิ้นงานบท Taxonomy และ Prioritization |
| docs/srs/use-cases.md, UC-07.md | use case 13 รายการ UC-07 fully dressed use case แบบ brief story | ชิ้นงานบท Stories |
| docs/srs/business-rules.md, booking.feature | BR-01 ถึง BR-05 Decision Table AC-07-01 ถึง AC-07-10 | ชิ้นงานบท Stories |
| docs/srs/traceability.md | ตามรอย EV ถึง AC | ชิ้นงานบท Stories |
| docs/srs/models.md, data-dictionary.md, cc-log.md, glossary.md | Model Set ทั้งหมด CC-01 ถึง CC-08 glossary | ชิ้นงานบท Modelling |
| docs/srs/questions.md | Q และ AS ทุกข้อพร้อมเจ้าของและพฤติกรรมชั่วคราว | ทุกบท |
| docs/srs/ai-prompt-log.md | บันทึกการใช้ AI #1 ถึง #11 | ทุกบท |

## งานของบทนี้ที่นักศึกษาต้องทำต่อ

บทเรียน Modern Specification และ SDD รวมทุกอย่างในนี้เป็นสเปกชุดเดียว แล้วประกาศ Baseline B1

1. ปิด Contradiction ใน cc-log.md ให้หมด และเพิ่ม REQ ที่มาจากโมเดลเข้า catalogue (สถานะ Draft)
2. เขียน spec.md ของ feature การจอง (UC-07) ครบ 11 ส่วน ส่วน Requirements ใส่รหัสกับสรุปสั้นเท่านั้น
3. เขียน intent.md ไม่เกิน 10 บรรทัด
4. เขียน plan.md (P-xx อย่างน้อย 4 ข้อ พร้อมทางเลือกที่ปฏิเสธ) และ tasks.md (T-xx อย่างน้อย 8 รายการ) ด้วยมือ แล้วตรวจสองทาง
5. แลกไฟล์กับกลุ่มข้างเคียง ไล่ task ย้อนถึง EV
6. เขียน Baseline Record BL-01 ให้เจ้าของความต้องการรับรอง แล้วติด tag B1
7. เขียน SRS แบบสารบัญตามโครง ISO/IEC/IEEE 29148 ที่ชี้ไปไฟล์จริง

ผลลัพธ์ของทุกข้ออยู่ใน repo ถัดไป **baanprom-sdd-02-build**
ทำของตัวเองก่อน แล้วค่อยเปิดเฉลย

## ถ้าทำของตัวเองพลาดหรือไม่ทัน

เอา repo นี้ไปทำต่อได้สองทาง

ทางที่ 1 บน GitHub

- เปิดหน้า repo นี้ กด Use this template แล้วเลือก Create a new repository
- ตั้งชื่อ repo ของกลุ่ม แล้วแก้ไฟล์ใน docs/srs/ ให้เป็นของกลุ่มเอง

ทางที่ 2 clone แล้วเปลี่ยน remote

```
git clone https://github.com/ppsajja/baanprom-sdd-01-spec.git baanprom-group
cd baanprom-group
git remote set-url origin https://github.com/<บัญชีของกลุ่ม>/<ชื่อ repo ของกลุ่ม>.git
git push -u origin main
```

`git remote set-url origin` เปลี่ยนปลายทางของ push จาก repo ของผู้สอนเป็น repo ของกลุ่ม (ต้องสร้าง repo เปล่าบน GitHub ไว้ก่อน)

## ทีม

- ชื่อทีม: กลุ่ม X (ตัวอย่างของรายวิชา)
- สมาชิก: สมาชิก A, สมาชิก B, สมาชิก C, สมาชิก D

## โครงของ repo

```
README.md                      ไฟล์นี้
docs/srs/README.md             ดัชนีไฟล์ต้นฉบับ บอกว่าแต่ละไฟล์มาจากบทไหน
docs/srs/problem-statement.md  ปัญหา ขอบเขต คุณค่าของลูกค้า
docs/srs/stakeholders.md       ทะเบียนผู้มีส่วนได้เสีย
docs/srs/evidence.md           ทะเบียนหลักฐาน
docs/srs/catalogue.md          บัญชีรายการความต้องการ
docs/srs/decisions.md          การจัดลำดับ แผนรุ่น และ Decision Record
docs/srs/use-cases.md          use case ทั้งระบบ และ story
docs/srs/UC-07.md              UC-07 fully dressed
docs/srs/business-rules.md     กฎธุรกิจ BR-01 ถึง BR-05
docs/srs/booking.feature       เกณฑ์การยอมรับของ UC-07
docs/srs/traceability.md       ตารางตามรอย
docs/srs/models.md             Model Set (Mermaid)
docs/srs/data-dictionary.md    พจนานุกรมข้อมูล
docs/srs/cc-log.md             บันทึกตรวจความสอดคล้อง
docs/srs/glossary.md           คำศัพท์กลาง
docs/srs/questions.md          คำถามเปิดและสมมติฐาน
docs/srs/ai-prompt-log.md      บันทึกการใช้ AI
```

## วิธีรัน

ยังไม่มีโค้ด เปิดอ่านไฟล์บน GitHub ได้เลย ภาพ Mermaid ใน models.md แสดงผลบน GitHub เอง

## สิ่งที่รู้อยู่แล้วว่ายังไม่ใช่ของจริง

- ตัวเลขทุกตัวเป็นตัวเลขสมมติเพื่อการสอน
- catalogue เต็มของกลุ่มมี REQ Approved 23 ข้อ แต่ไฟล์นี้มีเฉพาะข้อที่หน้าบทเรียนแสดง
- EV ที่หน้าบทเรียนไม่ได้แสดงไม่อยู่ในทะเบียน (ดูหมายเหตุท้ายตารางใน evidence.md)
- UC-03 fully dressed และ AC-03-01..04 (ตามที่ baseline เขียน) อยู่ในชุดงานของกลุ่ม แต่ไม่อยู่ในชุด repo นี้
- ข้อความบางส่วนเรียบเรียงขึ้นเพื่อให้ชุด repo ต่อเนื่อง ทุกจุดมีหมายเหตุกำกับในไฟล์

## คำถามที่ยังเปิด และจะได้คำตอบใน repo ไหน

| คำถาม | เรื่อง | ใน repo ถัดไป |
|---|---|---|
| Q-14 | BR-01 R3 ยกเลิกขณะช่างเดินทาง คืนเท่าไร (DR-02 ยังเสนอ) | ยังเปิด ประกาศพร้อม Baseline B1 ใน baanprom-sdd-02-build |
| Q-18 | ระยะล็อกช่วงเวลา | ยังเปิดใน baanprom-sdd-02-build คำตอบชั่วคราวมาตอน /clarify ใน baanprom-sdd-03-vv |
| Q-19 | gateway-timeout ตามสัญญา | ยังเปิด ใช้ 30 วินาทีชั่วคราว |
| Q-20, Q-22 | Technician.rating และ geoPoint | ยังเปิด ประกาศพร้อม Baseline B1 |
| CC-02, CC-05, CC-06, CC-07 | CC ที่ยังเปิด | ประกาศพร้อม Baseline B1 ใน baanprom-sdd-02-build |
| UC-08, UC-09 เข้า R1 ไหม | แผนรุ่นยังรอ SH-01 | ตัดสินในรอบ R1 release ของ baanprom-sdd-04-ops |
