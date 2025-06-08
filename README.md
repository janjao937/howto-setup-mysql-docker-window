# howto-setup-mysql-docker-window
howto-setup-mysql-docker-window

# (window search) Window feature on and off => virtual machine platform
- เปิด docker ใช้ได้ | MySQL ในเครื่องจะใช้ไม่ได้
- ปิด docker ใช้ไม่ได้ | MySQL ใช้ได้

# check MySQL ในเครื่อง
- Get-Service | Where-Object {$_.DisplayName -like "*MySQL*"}

Status   Name               DisplayName
------   ----               -----------
Stopped  MySQL80            MySQL80

*ต้องทำทุกครั้งถ้าจะใช้ MySQL ผ่าน docker เพราะ หลังเปิดเครื่อง  MySQL จะ auto running
# run cmd as admin ปิด/เปิด 
- net stop MySQL80
- net start MySQL80

# mysql ต้อง run 3306 เท่านั้น map ก็ไม่ได้


======
# อยากใช้ MySQL-docker
- (window search) Window feature on and off => virtual machine platform => เช็คถูก
- run cmd as admin ใช้ => net stop MySQL80 

=========
# อยากกลับมาใช้ MySQL ในเครื่อง
- (window search) Window feature on and off => virtual machine platform  => เอาเช็คถูกออก
- run cmd as admin ใช้ => net start MySQL80
