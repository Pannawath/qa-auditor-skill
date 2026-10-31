# Product Inspector (Universal QA & Quality Audit Skill)

AI Agent Skill สำหรับสวมบทบาทเป็น **"ผู้ตรวจคุณภาพผลิตภัณฑ์และโค้ดก่อนเผยแพร่" (Pre-Release Quality & UX Inspector)** รองรับทั้งเว็บไซต์ (Web Apps), โปรแกรมซอฟต์แวร์/เดสก์ท็อป (Software/Apps), โปรแกรม Command-Line (CLI Tools), และ API Services

---

## จุดเด่นของ Skill

1. **Grill-Me Onboarding**: สัมภาษณ์และคัดกรองข้อมูลก่อนเริ่มงานแบบ interactive multiple-choice
2. **Universal Scope**: ปรับเปลี่ยนหัวข้อการตรวจให้เหมาะกับลักษณะโปรเจกต์ (เว็บ, แอป, CLI, API)
3. **5 กลุ่ม 20 จุดตรวจครอบคลุม**:
   - **กลุ่ม A**: ความสม่ำเสมอของดีไซน์และอินเทอร์เฟซ (Design System, Typography, Spacing, Visual Hierarchy)
   - **กลุ่ม B**: ความยืดหยุ่นและการตอบสนองต่อสภาพแวดล้อม (Responsiveness, Overflow, Ergonomics, Font Scaling)
   - **กลุ่ม C**: สถานะการทำงานและการแจ้งเตือน (Loading, Empty States, Validation Feedback, Modals)
   - **กลุ่ม D**: การจำลองการใช้งานจริง (Critical User Journey, Dead Links, Keyboard Accessibility)
   - **กลุ่ม E**: ความพร้อมก่อนเผยแพร่ (Value Proposition, CTA Focus, Metadata & Asset Completeness)
4. **Strict Safety Guardrails**:
   - รอบแรกตรวจอย่างเดียว ห้ามแก้ไขไฟล์ ห้าม deploy
   - แยก "ตรวจพบจริง" ออกจาก "ข้อเสนอแนะ"
   - หยุดรอคำสั่ง **"อนุมัติให้แก้"** ก่อนลงมือแก้ไฟล์จริงเสมอ

---

## โครงสร้างไฟล์ใน Repository

```
qa-auditor-skill/
├── README.md
└── skills/
    └── product-inspector/
        └── SKILL.md
```

## การติดตั้งและการใช้งานใน Antigravity / Gemini CLI

คัดลอกโฟลเดอร์ `product-inspector` ไปไว้ที่โฟลเดอร์ skills ของคุณ:

- **Windows**: `%USERPROFILE%\.gemini\config\skills\product-inspector\SKILL.md`
- **macOS / Linux**: `~/.gemini/config/skills/product-inspector/SKILL.md`

เรียกใช้งานด้วยการพิมพ์คำสั่งตรวจโปรเจกต์ หรืออ้างอิง `@product-inspector`
