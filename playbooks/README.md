## Các playbook trong repo

### `deploy-webserver.yaml`

Playbook cài đặt stack LEMP (Nginx, MySQL/MariaDB, PHP) lên máy chủ target.

Các variable cần được define khị chạy (có thể được mã hoá bởi vault) bao gồm:

- `db_user`
- `db_passwd`
- `db_root_passwd`
- `wordpress_install_dir`
- `wordpress_db`
- `wordpress_hostname`
- `wordpress_http_port`

### Folder `secret/` chứa các file secret đã được mã hoá

### Folder `secret_examples/` chứa các file secret chưa được mã hoá. Các file này có thể được mã hoá qua `ansible-vault`

### Để chạy notebook với secret được mã hoá, sử dụng câu lệnh `ansible-playbook -i <inventory> --ask-vault-pass <playbook>`
