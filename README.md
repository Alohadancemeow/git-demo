# git-demo

git-demo

this line from remote repository.

this line from local repository.


## Git command :

>### git init

init คือ “intialize” คือเริ่มต้น ก่อนที่เราจะใช้งาน git ได้ต้อง git init (เราเป็นสร้าง repo คนแรก) เรามี Folder Project แล้วก็ทำการ git init จากนั้น git ก็จะมาคุม Project เราเรียบร้อยโดยค่าเริ่มต้นมันอยู่ที่ branch master.

>### git clone

clone คือ การเอางานที่เราต้องการลงมาไว้ที่เครื่องเรา (ใช้กรณีที่ไม่เคยมี Repository นั้นมาก่อน)

>### git status

status คือ ตรวจสอบสถานะของแฟ้ม ถ้ามีการเปลี่ยนแปลงก็จะแสดงให้เราเห็นว่ามีการแก้ที่ไหนหรือมีการลบที่ไหนออก ก่อนที่เราจะทำการใช้ git add ลำดับถัดไป

>### git add

add คือ เพิ่มไฟล์ที่มีการเปลี่ยนแปลงก่อนเพื่อจะ commit เหมือนประมาณว่าแพ็คของว่าจะเอาอะไรใส่กล่องบ้างโดย git add จะแบ่งเป็น 2 แบบดังนี้

>### 1. git add [path] 

หมายถึง ต้องการแอดเฉพาะไฟล์นั้นๆตามพาธที่เราต้องการเลือกทีละไฟล์เพื่อแพ็ค(unstage -> stage)ก่อนจะ commit อีกครั้ง

>### 2. git add . 

หมายถึง ต้องแอดทั้งหมดที่มีการเปลี่ยนแปลงเพื่อแพ็ค(unstage -> stage)ก่อนจะ commit อีกครั้ง

>### git commit

commit คือ เริ่มเก็บประวัติของแฟ้มต่าง ๆ ในโปรเจคโดยตอนนี้จะยังอยู่ใน Local Repository ส่วน -a หมายถึง All คือทั้งหมดที่มีการเปลี่ยนแปลง ส่วน -am ทั้งหมดและต้องการใส่คอมเม้นข้อความด้วย

>### git push origin [branch name]

push คือ การส่ง commit ที่ Local Repository ไปยัง Remote Repository

>### git pull origin [branch name]

pull คือ การดึง Remote Repository ไฟล์มายัง Local Repository เพื่อทำการอัพเดต โดยหลักๆที่จะเจอคือ pull มาแล้วทำงานต่อได้เลยและอีกแบบ pull มาแล้วเกิดการ merge และอาจจะเกิด conflict file กันซึ่งเราก็ต้องทำการแก้ไฟล์ที่ error แจ้งมาจะบอกว่าไฟล์อะไรบ้างที่มีการ conflict

>### git switch [branch name] 

ใช้กับ git version 2.23.0 last only

>### git checkout [path] or [branch name]

checkout คือ แปลตรงตัวเน้อคือต้องการออกจากอะไรก็ checkout ยกตัวอย่างในการใช้คำสั่งนี้ checkout branch กรณีที่ต้องการไปที่ branch อื่น

>### git merge [branch name]

merge คือ รวม เช่นเราทำงานที่ Branch develop ต้องการเอาไปรวมที่ Branch master ในการ merge ให้ทำการ checkout ไปที่ master และค่อยใช้ git merge develop เป็นต้น

>### git fetch 

คือ ใช้ดึงความเปลี่ยนแปลงจาก Remote Repository มายัง Local Repository

>### git stash

stash คือ การบันทึกการเปลี่ยนแปลงของเราไว้ก่อนและสามารถที่จะ restore กลับได้ทุกเมื่อ โดย stash จะแบ่งออกที่ใช้หลักๆ 4 คำสั่งดังนี้

>### 1. git stash save “[comment message]”

สำหรับบันทึกการเปลี่ยนแปลงลงในแฟ้ม stash ไว้ก่อน

>### 2. git stash pop [index] 

คือ การเอา stash list index ที่ต้องการเอาออกมา เป็นการเปลี่ยนแปลงเพื่อแก้ไขหรือทำงานต่อ

>### 3. git stash list 

คือ การแสดง stash list ที่เก็บไว้ทั้งหมด ❗️❗️ หมายเหตุ ออกจากการดู list ใช้ [control + z]

>### 4. git stash drop [index]

คือ ลบ stash list ออกสามารถเลือกลบโดยใส่ index ที่ต้องการได้เลย


### อ้างอิง :
[Medium](https://medium.com/trueid-developers/%E0%B9%80%E0%B8%A3%E0%B8%B4%E0%B9%88%E0%B8%A1%E0%B9%83%E0%B8%8A%E0%B9%89-git-command-line-%E0%B8%89%E0%B8%9A%E0%B8%B1%E0%B8%9A%E0%B8%A3%E0%B8%A7%E0%B8%9A%E0%B8%A3%E0%B8%B1%E0%B8%94%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B9%83%E0%B8%99-5-%E0%B8%99%E0%B8%B2%E0%B8%97%E0%B8%B5-e871be9807eb
)
