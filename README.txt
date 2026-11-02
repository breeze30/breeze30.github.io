พรทิพย์ กรุดเพชร — Portfolio (เว็บหน้าเดียว)
=================================================

ไฟล์ในโฟลเดอร์นี้
- index.html   หน้าเว็บพอร์ต (ไฟล์เดียวจบ ไม่ต้องติดตั้งอะไร)
- img/         รูปผลงานทั้ง 16 งาน
- print.html   เวอร์ชันสำหรับทำ PDF (เปิดในเบราว์เซอร์แล้ว Print → Save as PDF, กระดาษแนวนอน, ไม่มีขอบ)

วิธีเอาขึ้นเว็บฟรี (เลือกอย่างใดอย่างหนึ่ง)
1) Netlify Drop — ง่ายสุด ไม่ต้องสมัครก็ลองได้
   เปิด https://app.netlify.com/drop แล้วลากทั้งโฟลเดอร์นี้ไปวาง จะได้ลิงก์ทันที
   (สมัครฟรีถ้าอยากตั้งชื่อลิงก์เอง เช่น pornthip-portfolio.netlify.app)

2) GitHub Pages
   - สร้าง repo ใหม่ (public) ชื่ออะไรก็ได้ เช่น portfolio
   - อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้เข้า repo (index.html ต้องอยู่ระดับบนสุด)
   - Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save
   - รอ 1–2 นาที จะได้ลิงก์ https://<ชื่อผู้ใช้>.github.io/portfolio/

3) Vercel
   เปิด https://vercel.com/new → Import หรือลากโฟลเดอร์นี้วาง → Deploy

วิธีแก้ไขเนื้อหา
- เปิด index.html ด้วยโปรแกรมแก้ข้อความอะไรก็ได้ (VS Code, TextEdit)
- เลื่อนลงไปท้ายไฟล์ จะเจอบล็อก PROFILE (ชื่อ, ตำแหน่ง, อีเมล) และ CATEGORIES (รายการผลงาน)
- เพิ่มรูปให้โปรเจกต์: วางรูปใน img/ แล้วเพิ่มชื่อไฟล์ใน images: ["img/a.jpg", "img/b.jpg"]
  รูปแรกจะเป็นรูปหน้าปก ที่เหลือดูได้ใน lightbox (กดลูกศรหรือปัด)
- ใส่ role / stack / year / link ให้โปรเจกต์ได้ตามต้องการ ไม่ใส่จะไม่แสดง เช่น
  { name: "BLMS", desc: "...", role: "Mobile Developer", stack: "React Native", year: "2025",
    link: "https://...", linkLabel: "App Store", images: ["img/blms.jpg"] }
