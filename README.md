# final_part_1
1.ส่วนตัวผมมองว่า ถ้าเราจะใช้แต่กระบวนการ waterfall อย่างเดียวก็เป็นไปไม่ได้ เพราะ waterfall เองเป็นการทำงานแบบ มีขั้นตอน เมื่อมีการแก้ไขก็ไม่ามารถกลับไปแก้ไขได้ และยังใช้เวลาในการทำที่นานของแต่ละชั้น  เพราะฉะนั้นแแล้วในการ พัฒนาแอป บางอย่างก็ต้องอาศัย กระบวนการ agile เข้ามาช่วยเพื่อสะดวก รดวเร็ว ต่อการพัฒนา

2.ส่วนตัวผมคิดว่า การทำ version control สามารถใช้ได้ทั้ง 2 อย่าง ทั้ง git&github หรือ CVS หรือ SVN เพราะ ทั้งสองตัวนี้มีการทำงานที่แตกต่างกัน เพราะ SVN นั้น จะเรียกว่าการ Commitงจากที่ commit ไปแล้วไฟล์เหล่านั้นก็จะอยู่ใน repository ทันที ถ้าเป็น git การ commit จะเป็นการเก็บอยู่ใน local ก่อน แล้วค่อยๆ commit ทีละส่วน แล้วค่อย push ขึ้น repository ก็ได้

3.git init
  ->git add feature1 
  ->git commit -m "work feature1" 
  ->git push origin master

4.ใช่ ในการ merge ทุกครั้งต้องมีการเกิดการ conflict แน่นอน เพราะ เป็นการนำเอาโค้ดของคนในทีมมาแปะไว้ที่เดียวกัน เมื่อทำการ merge ก็จะเกิด conflict เสมอ 

5.'abcde' 

6.ในยุคสมัยนี้ เทคโนโลยีมันก้าวไกล คือทุกคนต้องใช้เทคโนโลยีเป็นใครใช้ไม่เป็นก็ถือว่าเชยมาก ในการทำ web application ขึ้นมาเพื่อเป็นการช่วยให้คนที่ใช้สมาร์ทโฟนหรือเทคโนโลยีต่างๆ สามารดาวน์โหลดหรือใช้งานได้สะดวก รวดเร็วไม่ว่าอยู่ที่ไหน

(7).1.เมื่อ user มีการร้องขอผ่าน view
  2.ข้อมูลจะส่งผ่านไปหา controller โดย controller จะเป็นตัวจำแนก action ต่างๆ หรือเป็น business logic ของระบบ
  3.จากนั้น controller ก็จะร้องขอไปยัง model จาก action นั้นๆ 
  4.เมื่อ model รับการร้องขอก็จะทำการ query ข้อมูลตามที่ controller ส่งมา
  5.model จะส่งข้อมูลที่ได้กลับมาหา controller
  6.controller ก็จะทำการ Sset ค่าลงในตัวแปรเพื่อส่งให้ view ต่อไป
  7.view ก็จะนำตัวแปรเหล่านั้นไปทำการแสดงผลตามต้องการได้

8.ตัวอย่าง framework ที่ใช้ คือ CodeIgniter 
framework เป็นขอบเขตของระบบงาน ที่เป็นรูปแบบที่นำกลับมาใช้ใหม่ได้สำหรับระบบซอฟต์แวร์ (หรือระบบย่อย) ซึ่งสามารถอยู่ในรูปของคลาสนามธรรม (Abstract class) และกับวิธีในการใช้ตัวตน (instance) ของคลาสร่วมกันจำเพาะสำหรับซอฟต์แวร์ชนิดใดชนิดหนึ่ง โครงร่างซอฟต์แวร์ทุกโครงร่างใช้การออกแบบเชิงวัตถุ
rails  เป็นการเผยแพร่ ผ่าน RubyGem เป็นตัวจัดการ Package ในภาษา Ruby ที่จะดูในเรื่องของ รูปแบบของ packaging และมี Libraries ไว้ให้ใช้มากมาย และมีโครงสร้าง ตัวช่วยในการทำงานมากมาย
ข้อดี framework 1.รวดเร็ว 2.ทำงานเป็นทีมได้ 3.เหมาะกับองค์กรใหญ่ ๆ
ข้อเสีย framework 1.ทุกสิ่งทุกอย่างมีดีย่อมมีเสียเสมอ ยิ่งมีประโยชน์มาก ยิ่งมีโทษมากเช่นกัน 2.มีขนาดของ source โดยรวมใหญ่กว่าที่ควรจะเป็น เพราะบางอย่างเราไม่จำเป็นต้องใช้ แต่ว่ามันดันมีใน Framework
ข้อดี rails 1.Code สั้น ดังนั้นโอกาสการเกิด Bug จึงน้อย การทำงานเป็นขั้นตอน สามารถแก้ไขได้ตรงจุด 2.เป็น Open source ของดีแถมฟรีด้วย 3.มี Library ให้นำไปใช้เป็นจำนวนมาก

9.Heroku คือ Platform as a Service (Paas) ที่ให้เราใช้งานได้ฟรี และมีแบบเสียเงินด้วย โดยรองรับภาษาโปรแกรมที่หลากหลาย เพื่อพัฒนา web applicationบทบาทหน้าที่ของ  Heroku คือ ช่วยให้การพัฒนา web application ของเราเป็นไปได้ง่าย และสะดวก เพราะ heroku รองรับภาษาของโปรแกรมที่เยอะและหลากหลายและเหมาะกับการใช้งานกับทุกคน ทั้งนักศึกษา บริษทั เป็นต้น

10.ที่มีสาขาวิชานี้เข้ามาในหลักสูตร เพราะในอนาคตต่อไปเรื่อยๆ เทคโนโลยีจะเข้ามามีบทบาทกับผู้คนมากขึ้น จึงทำให้คนต้องมีการเรียนรู้ที่จะพัฒนาซอฟต์แวร์ เพื่อรองรับสิ่งใหม่ที่จะเกิดขึ้นในอนาคต เพราะบางสิ่งห็ต้องมีการอัพเดทอยู่เสมอ เพื่อความทันสมัย จึงทำให้มีวิชา software davelopment process ขึ้นมาเพื่อเรียนรู้วิธีการพัฒนา ซอฟต์แวร์ 
