# Ansible-notebooks

## Tìm hiểu về ansible, cấu trúc playbook, cách hoạt động làm việc

Ansible là phần mềm giúp tự động hoá việc khởi tạo, cấu hình và triển khai phần mềm theo mô hình infrastructure-as-code

Ansible sử dụng yaml, json hoặc ini cho các file playbook, inventory, config và jinja2 cho các template

Ansible sử dụng kết nối tạm thời và chạy các module ngay trên node được điều khiển mà không cần sử dụng các daemon qua các phương thức kết nối ví dụ như ssh. Quá trình chạy của Ansible được giám sát bằng các phản hồi qua json đến máy điều khiển.

Một playbook của Ansible gồm có các thành phần chính:

- Các node cần điều khiển (được filter từ inventory)
- Các task hoặc role được thực hiện cho các node đó

Các dữ liệu nhạy cảm trong ansible có thể được mã hoá qua `ansible-vault`
