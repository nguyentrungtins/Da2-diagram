sequenceDiagram
    participant Client
    participant Auth
    participant Booking
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Booking: Tìm kiếm booking
    Booking->>+Booking: Xử lý yêu cầu tìm kiếm
    Booking-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUc9KwzAYf5WPXF1fIIeBztsuoh6G9BLT2IY2SZcmgzF2EJ9DUDwIoqDebJEdAr5H3mSpXZ1jyyXJL78_35dvgahKGMKoYlPLJGWnnKSaiFhCWCXRhlNeEmlgVHAmzT5-bE22j54olXOZ7j-cq4KdMS14VXElRxmjeSw7WpcQDYdHrSeGiXukYDLffFCQ6c-7b-45JO6rt21ZLfuAJYYx982dAKMJzAgPu_uEmXuAqZ375naTeEAZBceoyx_7emWCwNdPkP_Z7WZv-sRw6V5Fy6pXAq7_N79h7JAnvnmDwn3D3L1YoL5-tmC2BrvCtqDua0KK_i1mWxgaIBEaIDwJM1y0whiZjAkWIxyOCdF5jGK5DDxijbqYS4qw0ZYNkC0TYvp5I3xDiiqgYUhXSvX35RpPLc-t?type=png)](https://mermaid.live/edit#pako:eNptUc9KwzAYf5WPXF1fIIeBztsuoh6G9BLT2IY2SZcmgzF2EJ9DUDwIoqDebJEdAr5H3mSpXZ1jyyXJL78_35dvgahKGMKoYlPLJGWnnKSaiFhCWCXRhlNeEmlgVHAmzT5-bE22j54olXOZ7j-cq4KdMS14VXElRxmjeSw7WpcQDYdHrSeGiXukYDLffFCQ6c-7b-45JO6rt21ZLfuAJYYx982dAKMJzAgPu_uEmXuAqZ375naTeEAZBceoyx_7emWCwNdPkP_Z7WZv-sRw6V5Fy6pXAq7_N79h7JAnvnmDwn3D3L1YoL5-tmC2BrvCtqDua0KK_i1mWxgaIBEaIDwJM1y0whiZjAkWIxyOCdF5jGK5DDxijbqYS4qw0ZYNkC0TYvp5I3xDiiqgYUhXSvX35RpPLc-t)