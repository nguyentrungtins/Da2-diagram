sequenceDiagram
    participant Client
    participant Auth
    participant Port
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Port: Cập nhật cảng
    Port->>+Port: Xử lý yêu cầu cập nhật
    Port-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptkcFKwzAYx1_lI1fXF8hhIPO2y1APQ3IJaWxD26RLk0EZO4jPISgeBGGg3mwRDwXfI29isq6bsvXQpF9____3T74VYirmCKOKLyyXjF8ImmhaEAn-Kak2gomSSgOTXHBpjuvn1qTH1ZnSJ9hLlfMZ14WoKqHkJOUsI7LHevtoPD4Lhhjm3RMDk7r2nYFMft5c-yAg7j5l0vOBCvQJSwxT4dr7AoymsKTCr90HLLtHWNjatXe7jieUkXeM-v5T13wbL3DNM2R7u_-9wyExTFyzKUGmfjHAPD9EDL8P2Ny1G8i7L6i7Vxu4l-17L_2jCSn6-8BwrbcJDmmIRCNU-NxUxH5uq6AjyKS84ARhv42pzggicu05ao26qiVD2GjLR8iWMTXDjBG-pXnlq342N0oN3-tfAv_M1A?type=png)](https://mermaid.live/edit#pako:eNptkcFKwzAYx1_lI1fXF8hhIPO2y1APQ3IJaWxD26RLk0EZO4jPISgeBGGg3mwRDwXfI29isq6bsvXQpF9____3T74VYirmCKOKLyyXjF8ImmhaEAn-Kak2gomSSgOTXHBpjuvn1qTH1ZnSJ9hLlfMZ14WoKqHkJOUsI7LHevtoPD4Lhhjm3RMDk7r2nYFMft5c-yAg7j5l0vOBCvQJSwxT4dr7AoymsKTCr90HLLtHWNjatXe7jieUkXeM-v5T13wbL3DNM2R7u_-9wyExTFyzKUGmfjHAPD9EDL8P2Ny1G8i7L6i7Vxu4l-17L_2jCSn6-8BwrbcJDmmIRCNU-NxUxH5uq6AjyKS84ARhv42pzggicu05ao26qiVD2GjLR8iWMTXDjBG-pXnlq342N0oN3-tfAv_M1A)