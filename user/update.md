sequenceDiagram
    participant Client
    participant Auth
    participant User
    participant Role
    participant Permission
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+User: Cập nhật thông tin người dùng
    User->>+User: Xử lý yêu cầu cập nhật thông tin người dùng
    Auth->>+Role: Cập nhật vai trò của người dùng
    Role->>+Role: Xử lý yêu cầu cập nhật vai trò
    Auth->>+Permission: Cập nhật quyền của người dùng
    Permission->>+Permission: Xử lý yêu cầu cập nhật quyền
    Auth->>+RolePermissionCheck: Kiểm tra quyền và vai trò của người dùng
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    User-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqNU91KwzAYfZWP3Lq9QC4EmXe7EX9gSG9CGtuwNu3SdDDGLsTnEBQvBsJAxRtbxIuA75E3MVnXVdvh1os2PT3nfKdfvswRTXyGMMrYJGeCslNOAkliT4C9UiIVpzwlQsEg4kyoLn6Sq7CLXmVMdtHzJGJd9IzJmGcZT8RuRfN9EDI69ja0KlD_-PjIRcAw0o8UVGjKVwoi-H4x5T0HX3-IoOI7lmO7aBgGplilIEL7UFal30UAioudSqdolCNTriDSnzDTzzlQUyzX94Pd6hzu11o5poSDkvrN-pVLslPtVI16b5ba8W_ppqOtAJN8Zspb8U_9Rto22ptlY97tQmuDMQy5Ke9iG5xsE031w6Htadn1bZl-NSJDU3y5HKZ4gvG2xq9NdtRqrjBcyjWtkXgC9VBszQn37YmZO52HVMhi5iFslz6RYw95YmF5JFfJxUxQhJXMWQ_lqU9UfboQviFRZlE749dJUr8vfgBW-XM4?type=png)](https://mermaid.live/edit#pako:eNqNU91KwzAYfZWP3Lq9QC4EmXe7EX9gSG9CGtuwNu3SdDDGLsTnEBQvBsJAxRtbxIuA75E3MVnXVdvh1os2PT3nfKdfvswRTXyGMMrYJGeCslNOAkliT4C9UiIVpzwlQsEg4kyoLn6Sq7CLXmVMdtHzJGJd9IzJmGcZT8RuRfN9EDI69ja0KlD_-PjIRcAw0o8UVGjKVwoi-H4x5T0HX3-IoOI7lmO7aBgGplilIEL7UFal30UAioudSqdolCNTriDSnzDTzzlQUyzX94Pd6hzu11o5poSDkvrN-pVLslPtVI16b5ba8W_ppqOtAJN8Zspb8U_9Rto22ptlY97tQmuDMQy5Ke9iG5xsE031w6Htadn1bZl-NSJDU3y5HKZ4gvG2xq9NdtRqrjBcyjWtkXgC9VBszQn37YmZO52HVMhi5iFslz6RYw95YmF5JFfJxUxQhJXMWQ_lqU9UfboQviFRZlE749dJUr8vfgBW-XM4)