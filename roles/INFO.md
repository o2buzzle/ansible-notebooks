## Về các roles trong Ansible

Một Role trong Ansible là một đơn vị chứa các biến, các task, handler, v.v nhằm phục vụ một mục đích nào đó.
Các role thường được sử dụng nhằm đơn giản hoá việc sử dụng lại và chia sẻ các task giữa nhiều playbook

Một role trong Ansible thường có các thành phần

- `tasks` - Danh sách các task trong role
- `handlers` - Các handler mà role cung cấp
- `templates` - Các file mẫu có thể được template bằng Jinja2
- `files` - Các file được role deploy
- `vars` - Các biến role sử dụng
- `defaults` - Các varible mặc định cho role
- `meta` - Các metadata của role
- `library` - Các module con trong role

Role thường được chứa trong folder `roles/` cùng với file Playbook, hoặc trong các folder mặc định của Ansible

Các role được sử dụng trong Ansible theo hình thức:

- Include cứng trong playbook

```yml
roles:
  - ../roles/wordpress
```

- Include dynamic trong một task

```yml
- name: Include the webserver role
      include_role:
        name: webserver
```
