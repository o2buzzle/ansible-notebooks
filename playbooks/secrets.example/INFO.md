## Mã hoá thông tin nhạy cảm với Ansible Vault

Trong một playbook hoặc các file vars thường có thể có các thông tin nhạy cảm (ví dụ mật khẩu root, db, v.v.)

Các giá trị này có thể được mã hoá các biến này khi lưu trữ nhằm tránh lộ lọt thông tin sử dụng Ansible Vault

Để sử dụng Ansible Vault, ta tạo file có nội dung là dữ liệu cần mã hoá.
Sau đó mã hoá bằng Ansible Vault

Khi mã hoá có thể cung cấp password trực tiếp hoặc sử dụng file password với vault id nếu cần nhiều password hơn cần thiết

Các giá trị được mã hoá có thể được chứa trong file riêng hoặc embed trong các file khác
