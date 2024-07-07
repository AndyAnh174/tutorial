# Hướng dẫn cách cài đặt SSH Key cho GitHub
#### [AndyAnh174](https://github.com/AndyAnh174/)

# Tại sao cần SSH K?? 🤔

Mã SSH key của GitHub được sử dụng để xác thực an toàn khi bạn kết nối và thao tác với kho lưu trữ GitHub thông qua giao thức SSH. Thay vì sử dụng phương thức xác thực bằng mật khẩu (password), bạn có thể sử dụng cặp khóa SSH để xác thực, bao gồm một khóa công khai và một khóa riêng tư.

Sau đây là cách cài đặt mã SSH key:

## Linux

`Bước 1`: Các bạn `Terminal` lên.

`Bước 2`: Các bạn nhập đoạn code như sau:
```sh
ssh-keygen -t ed25519 -C "your_email@example.com"
# Lưu ý: Nếu bạn đang sử dụng hệ thống cũ không hỗ trợ thuật toán Ed25519, hãy sử dụng:
# Ví dụ: ssh-keygen -t ed25519 -C "hovietanh147@gmail.com"
```
sau đó các bạn cứ nhấn Enter đến khi nào nó hiện như này là đúng 
![alt text](image-1.png)

`Bước 3`: Các bạn tiếp tục nhập cho mình đoạn code này:
```sh
cat ~/.ssh/id_ed25519.pub
# Sau đó chọn và sao chép nội dung
# hiển thị trong terminal vào clipboard của bạn
```
![alt text](image-2.png)

`Bước 4`: Các bạn vào trang github của các bạn (nhớ đăng nhập tài khoảng github trước khi vào), sau đó các bạn nhấn vào link này [tại đây](https://github.com/settings/keys).

`Bước 5`: Nó sẽ hiện ra giao diện như này.
![alt text](image-3.png)

Tiếp đó các bạn nhấn vào nút màu xanh `New SSH key`.
![alt text](image-4.png)

Nó sẽ hiển thị ra cái bảng add new key
![alt text](image-5.png)

Và giờ chúng ta sẽ quay về `Bước 3`để copy key hiện trong terminal add vào thôi, Đây là Ví Dụ:
![alt text](image-6.png)

Nó hiện như này là xong rồi đoóo :333
![alt text](image-7.png)

## Windows
