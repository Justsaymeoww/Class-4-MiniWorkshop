# **Class 4 - Mini Workshop**
### ขั้นตอนการทำ Mini Workshop

**1. Clone repository ลงในเครื่องตัวเอง**

**2. ใช้คำสั่งตามด้านล่างนี้**
- เช็คว่าในเครื่องมีการ login github ค้างไว้ไหม
```bash
git credential-manager github list
```

- log out ออกจากบัญชี (ในกรณีที่มีlog in ค้างไว้อยู่)
```bash
git credential-manager github logout <username>
```

- log in บัญชีตัวเอง
```bash
git credential-manager github login
```
- config ชื่อและอีเมล
```bash
git config --local user.name "Full name"
git config --local user.email "Your Email"
```
---
**3. สร้าง Branch แยกโดยตั้งชื่อตาม Format นี้**
```bash
git branch <ชื่อเล่นภาษาอังกฤษของตัวเอง> 
```
**4. เข้าไปใน Branch ที่เพิ่งสร้างมา**

**5. สร้างไฟล์ <ชื่อเล่นภาษาอังกฤษของตัวเอง>.md**
```bash
code .
```

**6. คัดลอก Format ตามด้านล่างนี้ลงไปในไฟล์.md**

```bash
## 💌 จดหมายถึงพี่ ๆ ในบ้าน Empire cache 💌

> เขียนจากใจ ไม่ต้องยาว ขอแค่จริงใจ 💜
> เพิ่มชื่อตัวเองและข้อความของตัวเองต่อท้ายในหัวข้อได้เลย


## 🧑‍💻 จากน้อง<เขียนชื่อเล่นตัวเองที่นี่>

- **ถึงพี่บ้าน Empire cache:**
  > _เขียนความรู้สึกที่นี่_

---
```

**7. แก้ไขตรงส่วนที่ให้เติมข้อความ**

**8. ใช้ Git Workflow ตามปกติ**
```bash
git add <name>.md
git commit -m "Add <name>.md file"
git push -u origin <ชื่อbranch>
```
*git push ใน branch ของตัวเองเท่านั้น ห้าม push ลง main

**9. Create Pull Request** จาก Branch ตัวเองลงที่ main

**10. รอ Approve**

**11. Merge Pull Request**
