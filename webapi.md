# Hoàn cảnh

Giả định rằng mình cần triển khai một web/app bán sách online, thiết kế và implement một hệ thống API Restful với các giai đoạn như sau

## Giai đoạn 1: Tạo basic các API CRUD dưới dạng public

### Book - Sách

- Id
- Name
- Description
- Price
- Year
- AuthorId
- Publisher
- Cover
- List<Category>

### Chủng loại - Category

- Id
- Name
- Description
- List<Book>

### Tác giả - Author

- Id
- Name
- Website
- Birthday
- Cover

Lưu ý về cover:

- Ảnh cover phải được lưu trên server vào 1 thư mục cố định được config từ file Web.config
- Ảnh cover phải được lưu dưới dạng <GUID>.<Extension>
- Ảnh cover phải được limit size tối đa là 800*800 (Server tự giảm kích thước file ảnh trước khi lưu)

## Giai đoạn 2: Tạo thông tin người dùng và phân quyền

### User

- Id
- Name
- Username
- Password
- Birthday
- List<Role>
- LastOnline


### Role

- Id
- Name
- Description

Có 3 role luôn được định nghĩa sẵn

- Admin: Quản lý người dùng (CRUD)
- Manager: Quản lý sách (Xem, chỉnh sửa, xoá sách)
- Contributer: Cộng tác viên (Thêm sách và chỉnh sửa sách của chính họ)

Ngoài ra, cả 3 role đó đều được phép đăng nhập, đăng xuất, xem, chỉnh sửa thông tin cá nhân (chỉ có admin mới được chỉnh role)

Sử dụng cơ chế JWT để đăng nhập