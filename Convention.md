Phiên bản đầy đủ: https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions

Sơ lược cần chú ý:

- Cách đặt tên: 
    - Tất cả đều là `UpperCase` ngoại trừ các trường hợp dưới đây là dùng `camelCase`
        - Biến private thuộc lớp (C# gọi là trường)
        - Biến/tham số của method, lambda
    - Không dùng prefix, postfix để cho biết kiểu biến

- String:
    - Dùng `string` thay vì `String`
    - Dùng [string interpolation](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/tokens/interpolated) thay vì các phép nối (+) chuỗi
    - Dùng `string.Equals` để kiểm tra 2 chuỗi bằng nhau

- Biến:
    - Dùng var để khai báo biến nếu có thể
    - Scope của biến càng nhỏ càng tốt
