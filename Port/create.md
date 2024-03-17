sequenceDiagram
    participant Client
    participant Auth
    participant Port
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Port: Tạo mới cảng
    Port->>+Port: Xử lý yêu cầu tạo mới
    Port-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptkUFKxDAUhq_yyNbpBbIYkHE3m0FdDJJNSGMb2iadNBkowyzEY4jg4EIQBHVni7goeI_cxMRaq8xkk-T1-___pW-DmIo5wqjiK8sl4yeCJpoWRIJfJdVGMFFSaWCWCy7Nfv3YmnS_ulD6AHuqcr7guhBVJZScpZxlRPZYbx9Np0fBEMOy2zEwqWtfGMjk89m1twLi7k0mPR-oQB-wxDAXrr0uwGgKayr83r3CuruDla1de_WTeEAZeceoz5-75sN4gWvuIfu1-58dHonh3DU7BYVrbwQwjw8dhq8jtXTtE-TdO9Tdow3cgwUzKv9IQg_93_De-jt_7IVINEGF75qK2E9tE3QEmZQXnCDsjzHVGUFEbj1HrVFntWQIG235BNkypmaYMMKXNK981U_mQqnhvv0CQUbL0g?type=png)](https://mermaid.live/edit#pako:eNptkUFKxDAUhq_yyNbpBbIYkHE3m0FdDJJNSGMb2iadNBkowyzEY4jg4EIQBHVni7goeI_cxMRaq8xkk-T1-___pW-DmIo5wqjiK8sl4yeCJpoWRIJfJdVGMFFSaWCWCy7Nfv3YmnS_ulD6AHuqcr7guhBVJZScpZxlRPZYbx9Np0fBEMOy2zEwqWtfGMjk89m1twLi7k0mPR-oQB-wxDAXrr0uwGgKayr83r3CuruDla1de_WTeEAZeceoz5-75sN4gWvuIfu1-58dHonh3DU7BYVrbwQwjw8dhq8jtXTtE-TdO9Tdow3cgwUzKv9IQg_93_De-jt_7IVINEGF75qK2E9tE3QEmZQXnCDsjzHVGUFEbj1HrVFntWQIG235BNkypmaYMMKXNK981U_mQqnhvv0CQUbL0g)