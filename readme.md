


Html:
<clipPath id="fillCM"> เอาไว้แก้ SVG path ของ mask น้ำ วิธีทำ svg น้ำ
*ไม่แน่ใจว่ากำหนดขนาดได้ไหม* ถ้ากำหนดได้ ขอ 300 x 300 px ทำเป็น SVG ก่อนแล้วเข้า aistudio.google.com ใช้คำสั่ง
แปลงเป็น svg path ให้หน่อย แล้ววาง code ของ svg ลงไป แล้วเอาไปแทนที่ใน <clipPath id="fillCM">

CSS:
ปรับแค่ .cm และ .front พยายามไม่แก้ width/height ให้ปรับ zoom กับ bottom/left แทน

.fill .fend เอาไว้กำหนดน้ำตอนต่ำสุด ไว้ด้านล่างของ logo พอดี โดยต้อง เอา /* */ ครอบส่วน   clip-path: url(#fillCM);  ใน .cm ก่อนถึงจะเห็นน้ำแบบเต็ม

๋JS:
แก้การเพิ่มของระดับน้ำได้ที่   goalRel = goalRel * 0.45; /* เพิ่มลดการเปลี่ยนแปลงระดับน้ำ ยิ่งเยอะ น้ำยิ่งเพิ่มขึ้นมาก */ (บรรทัดที่ 74)
ก่อนส่งมอบงานต้องทำการ encode เพื่อไม่ให้ลูกค้าเห็น หรือแก้ code ส่วนนี้ได้
decode ใช้ https://webcrack.netlify.app/
ส่วน encode ใช้ https://javascriptobfuscator.com/

data:
  "top": "https://i.imgur.com/YzgRWcv.png", ตรงนี้เอาไว้แก้รูป layer บนสุดของ widget