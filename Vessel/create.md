sequenceDiagram
    participant Client
    participant Auth
    participant Vessel
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Vessel: Tạo mới tàu
    Vessel->>+Vessel: Xử lý yêu cầu tạo mới
    Vessel-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUU1KAzEUvsojW9sLZFGQuutGVKRINiHz7ITOJG0mKZTShXgMEVpcCIKg7pxBXAS8R25ixlhrabNJ8s33l3kLInSGhJIKpw6VwBPJR4aXTEFcE26sFHLClYV-IVHZffzY2XwfvcSqwmIfP9MFnqIpZVVJrfo5ijFTiZYCur3eUWtJYejXAmwemlcBavT1Epp7CZl_V6PEb1kt-4AlhYEMzW0J1nCYcRl3_wYzv4Kpm4fm5jfxgLIbHbspfxDqTxsFoX6A8Z_dbnZ6JoWLUK81lKG5i1l-5RIrff3PG4bmGQr_AXP_5ECE-tGB3Wp3ZG2T9E-iv_lpsW3EFOmQMnbnMovTW7RKRmyOJTJC4zHjZswIU8vI487q87kShFrjsEPcJON2M2lCr3lRRTTO50rrzX35DXxZzqk?type=png)](https://mermaid.live/edit#pako:eNptUU1KAzEUvsojW9sLZFGQuutGVKRINiHz7ITOJG0mKZTShXgMEVpcCIKg7pxBXAS8R25ixlhrabNJ8s33l3kLInSGhJIKpw6VwBPJR4aXTEFcE26sFHLClYV-IVHZffzY2XwfvcSqwmIfP9MFnqIpZVVJrfo5ijFTiZYCur3eUWtJYejXAmwemlcBavT1Epp7CZl_V6PEb1kt-4AlhYEMzW0J1nCYcRl3_wYzv4Kpm4fm5jfxgLIbHbspfxDqTxsFoX6A8Z_dbnZ6JoWLUK81lKG5i1l-5RIrff3PG4bmGQr_AXP_5ECE-tGB3Wp3ZG2T9E-iv_lpsW3EFOmQMnbnMovTW7RKRmyOJTJC4zHjZswIU8vI487q87kShFrjsEPcJON2M2lCr3lRRTTO50rrzX35DXxZzqk)