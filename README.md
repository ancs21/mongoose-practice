# Mongoose-practice
MongoDB Practice with Mongoose ORM

### Mô hình quan hệ
#### Many to many
 
 Thiết kế lược đồ cho mô hình sau:
 - Một môn học có thể được học bởi nhiều học sinh
 - Một học sinh có thể học nhiều môn học
 
 Môn học (Course) gồm 2 fields là mã môn học (code), và tên môn học (name)
 Học sinh (Student) gôm 3 fields là họ (firstName), tên (lastName) và tuổi (age), đồng thời có 1 field (courses) tham chiếu đến danh sách các môn học
 
 REST API gồm các tính năng sau:
  - Trả về tất cả môn học (/api/courses)
  - Trả về tất cả học sinh (/api/students)
  - Tìm học sinh theo tên (/api/students/:name)
  - Tìm những học sinh học chung 1 môn học (/api/students/course/:idCourse)
  
 
