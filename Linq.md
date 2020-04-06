## Chuẩn bị:

Tạo các model sau:

### Class:
    - Id: int
    - Name: string

### Student:
    - Id: int
    - Name: string
    - Class: Class
    - Birthday: DateTime
    - Score: Double?

### DataFactory:
    - Students: List<Student>
    - Class: List<Class>

1. Viết hàm lấy về điểm của một student theo id 
2. Viết hàm lấy danh sách sinh viên sinh có năm sinh là year
3. Viết hàm lấy danh sách sinh viên theo tên theo tên lớp
4. Viết hàm lấy điểm trung bình của các sinh viên theo tên lớp
5. Viết hàm lấy danh sách sinh viên có điểm cao nhất của mỗi lớp. (Mỗi lớp lấy tối đa 1 người)
6. Viết hàm lấy danh sách sinh viên có tên chứa chuỗi X
7. Viết hàm lấy danh sách các điểm xuất hiện trong toàn bộ dữ liệu
8. Viết hàm lấy danh sách các sinh viên có điểm thấp hơn 5
9. Viết hàm lấy danh sách các sinh viên chưa có điểm
10. Viết hàm đếm lấy danh sách lớp kèm theo số sinh viên điểm cao hơn 8
11. Viết hàm tìm lớp có điểm trung bình cao nhất
12. Viết hàm lấy 5 sinh viên ngẫu nhiên của 1 lớp nào đó
13. Viết hàm kiểm tra xem lớp 10A có sinh viên nào đó sinh năm 2000 mà điểm >= 8 hay không (thay các giá trị bằng param)


14. Viết chương trình sắp xếp một list gồm các "Họ Và Tên" theo thứ tự tăng dần theo tên (rồi đến họ) của tiếng Việt

