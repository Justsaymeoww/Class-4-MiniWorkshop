# **Class 4 - Mini Workshop**
### ขั้นตอนการทำ Mini Workshop

**1. Fork repository และ Clone ลงในเครื่องตัวเอง**

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

**3. ตรวจสอบ/ตั้งค่า remote ในเครื่อง**

เช็คก่อนว่าตอนนี้ remote origin ชี้ไปที่ไหน:
```bash 
git remote -v
```
ถ้าเห็นว่าชี้ไปที่ repo ของพี่ (Justsaymeoww/...) ให้เปลี่ยนเป็น fork ของตัวเอง :
```bash 
git remote set-url origin https://github.com/<github_username>/Class-4-MiniWorkshop.git
```

เช็คอีกครั้งให้แน่ใจ:
```bash 
git remote -v
```
ควรเห็น:
```bash 
origin  https://github.com/<github_username>/Class-4-MiniWorkshop.git (fetch)

origin  https://github.com/<github_username>/Class-4-MiniWorkshop.git (push)
```


**4. สร้าง Branch แยกโดยตั้งชื่อตาม Format นี้**
```bash
git branch <ชื่อเล่นภาษาอังกฤษของตัวเอง> 
```
**5. เข้าไปใน Branch ที่เพิ่งสร้างมา**

**6. สร้างไฟล์ <ชื่อเล่นภาษาอังกฤษของตัวเอง>.md**
```bash
code .
```

**7. คัดลอก Format ตามด้านล่างนี้ลงไปในไฟล์.md**

```bash
## 💌 จดหมายถึงพี่ ๆ ในบ้าน Empire cache 💌

> เขียนจากใจ ไม่ต้องยาว ขอแค่จริงใจ 💜
> เพิ่มชื่อตัวเองและข้อความของตัวเองต่อท้ายในหัวข้อได้เลย


## 🧑‍💻 จากน้อง<เขียนชื่อเล่นตัวเองที่นี่>

- **ถึงพี่บ้าน Empire cache:**
  > _เขียนความรู้สึกที่นี่_

---
```

**8. แก้ไขตรงส่วนที่ให้เติมข้อความ**

**9. ใช้ Git Workflow ตามปกติ**
```bash
git add <name>.md
git commit -m "Add <name>.md file"
git push -u origin <ชื่อbranch>
```
*git push ใน branch ของตัวเองเท่านั้น ห้าม push ลง main

---

**10. เปิด Pull Request**

เข้าไปที่ fork ของน้องบน GitHub: 
https://github.com/<github_username>/Class-4-MiniWorkshop

**จะเห็นแถบสีเหลืองขึ้นมาว่า "<branch_name> had recent pushes" และกดปุ่ม Compare & pull request**

**ตรวจสอบให้แน่ใจว่า:**

base repository = Justsaymeoww/Class-4-MiniWorkshop, 

base branch = main (หรือ branch หลักที่เพื่อนใช้)

head repository = <github_username>/Class-4-MiniWorkshop, compare = <branch_name>


ใส่หัวข้อ/รายละเอียดงานที่ทำ
เช่น Title : Letter From Nong

กด Create pull request
