sequenceDiagram
    participant Client
    participant Auth
    participant Container
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Container: Cập nhật container
    Container->>+Container: Xử lý yêu cầu cập nhật
    Container-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUc1KAzEQfpUhV7svkENB1lsvoh6K5BKysRu6O9lmk0IpPYjPISgeBKGg3txFPCz4HnkTs912pT85ZJLJ9zOZWRKhE0koKeXMSRTyQvGJ4TlDCKvgxiqhCo4W4kxJtMf5c2fTE2iNliuU5vjpSmfyUppclaXSGKdSTBl2sM4jGg7PWlUK4-ZZgE19_SEAJ7_vvn5UkDRfOOnwLapFn5CkMFK-fsjBGg5zrkJsPmHePMHMLXx9v3U8wYyCYtT5j3z1YwPBVy8w7eX2vfufUoh9tS4A0xAsiP0O9LADztjXa8iab1g0bw6Er143e69zyG6L69pE4cZsCvsvkiEZkDx8h6skzHTZkhmxqcwlIzQcE26mjDBcBRx3Vl8vUBBqjZMD4oqE2938Cb3jWRmyYWS3Wu_uqz-OOdcX?type=png)](https://mermaid.live/edit#pako:eNptUc1KAzEQfpUhV7svkENB1lsvoh6K5BKysRu6O9lmk0IpPYjPISgeBKGg3txFPCz4HnkTs912pT85ZJLJ9zOZWRKhE0koKeXMSRTyQvGJ4TlDCKvgxiqhCo4W4kxJtMf5c2fTE2iNliuU5vjpSmfyUppclaXSGKdSTBl2sM4jGg7PWlUK4-ZZgE19_SEAJ7_vvn5UkDRfOOnwLapFn5CkMFK-fsjBGg5zrkJsPmHePMHMLXx9v3U8wYyCYtT5j3z1YwPBVy8w7eX2vfufUoh9tS4A0xAsiP0O9LADztjXa8iab1g0bw6Er143e69zyG6L69pE4cZsCvsvkiEZkDx8h6skzHTZkhmxqcwlIzQcE26mjDBcBRx3Vl8vUBBqjZMD4oqE2938Cb3jWRmyYWS3Wu_uqz-OOdcX)