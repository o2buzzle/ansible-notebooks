## Các role trong repo

### Common

Một số task được thực hiện chung cho các role

### lemp-stack

Cài stack LEMP (Nginx, MySQL, PHP) trên máy chủ Linux

Các varible cần được cung cấp:

- `db_root_passwd`

### wordpress

Cài Wordpress lên máy chủ (depend lên lemp)

Các varible cần được cung cấp:

- `db_user`
- `db_passwd`
- `wordpress_install_dir`
- `wordpress_db`
- `wordpress_hostname`
- `wordpress_http_port`
