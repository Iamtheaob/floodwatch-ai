# FloodWatch AI — พร้อม Deploy

แอปแจ้งเตือนน้ำท่วมและประเมินความเสี่ยงด้วย Machine Learning

## ไฟล์ในแพ็กเกจนี้

- `index.html` — ตัวแอป (ไฟล์หลัก)
- `manifest.json` — ไฟล์สำหรับติดตั้งแอปบนมือถือ (PWA)

## วิธี Deploy เร็วที่สุด (1 นาที)

1. ไปที่ <https://app.netlify.com/drop>
1. ลากทั้งโฟลเดอร์นี้ไปวางในกรอบ
1. รอ 15 วินาที — ได้ URL ใช้งานได้ทันที

## วิธีอื่นๆ

ดูคู่มือละเอียดในไฟล์ FloodWatch_Deploy_Guide.docx
ครอบคลุม Netlify, GitHub Pages, Vercel และการตั้ง custom domain

## ข้อควรรู้

- ต้อง deploy หรือรันผ่าน http/https เท่านั้น — เปิดไฟล์แบบ file:// จะดึงข้อมูลฝนจริงไม่ได้
- แอปใช้ Open-Meteo API (ฟรี ไม่จำกัด ไม่ต้อง API key)
- ถ้าดึงข้อมูลจริงไม่ได้ แอปจะใช้ข้อมูลจำลองอัตโนมัติ

## เทคโนโลยี

- HTML/CSS/JavaScript ล้วน ไม่มี dependency
- ML Model: Gradient Boosting Ensemble 7 trees
- แรงบันดาลใจจาก Kaggle Electricity Load Prediction 2026