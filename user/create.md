sequenceDiagram
    participant Client
    participant Auth
    participant User
    participant Role
    participant Permission
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+User: Tạo mới người dùng
    User->>+User: Xử lý yêu cầu tạo mới người dùng
    Auth->>+Role: Tạo mới vai trò cho người dùng
    Role->>+Role: Xử lý yêu cầu tạo mới vai trò
    Auth->>+Permission: Tạo mới quyền cho người dùng
    Permission->>+Permission: Xử lý yêu cầu tạo mới quyền
    Auth->>+RolePermissionCheck: Kiểm tra quyền và vai trò của người dùng
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    User-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqFU89qwjAYf5WPXKcv0IMw3M3L2B-Q0UtIMxtsE00TQcTD2GOMwWQHYTDYdlvD2KGw98ibmKzWqlXMqfn6-5cvX2aIiIiiAGV0rCkn9ILhgcRpyMGtEZaKETbCXEE3YZSrZv1cq7hZvc2obFavREKb1UsqU5ZlTPDDjPp_N6ZkGK5hZaB2p3PmIwTQLxYEVGzNJwE--Puw5plBVHzzQYn3KI_20QK4sflCQGrNEzuI9qga3bfmHZLiB6bFmwZi86UGdUKh8vNH2PWbYAZKFl9AYnGQ6ik19ZR5JbdrW3dt13ysp9Y88KPeNW9f5VSOtXLz9HsXGECPWfOYutB4E2dSvGz1xZolPtqZPbm2s2mXI9Cz-a9ykjZ_heHGY-tCPbScG9cU-Q-rKSFHLZQ6ccwi9yJmnhciFdOUhihwnxGWwxCFfO5wWCtxPeUEBUpq2kJ6FGFVvR4U3OMkc1U3w3dCVPv5Ch9pYzI?type=png)](https://mermaid.live/edit#pako:eNqFU89qwjAYf5WPXKcv0IMw3M3L2B-Q0UtIMxtsE00TQcTD2GOMwWQHYTDYdlvD2KGw98ibmKzWqlXMqfn6-5cvX2aIiIiiAGV0rCkn9ILhgcRpyMGtEZaKETbCXEE3YZSrZv1cq7hZvc2obFavREKb1UsqU5ZlTPDDjPp_N6ZkGK5hZaB2p3PmIwTQLxYEVGzNJwE--Puw5plBVHzzQYn3KI_20QK4sflCQGrNEzuI9qga3bfmHZLiB6bFmwZi86UGdUKh8vNH2PWbYAZKFl9AYnGQ6ik19ZR5JbdrW3dt13ysp9Y88KPeNW9f5VSOtXLz9HsXGECPWfOYutB4E2dSvGz1xZolPtqZPbm2s2mXI9Cz-a9ykjZ_heHGY-tCPbScG9cU-Q-rKSFHLZQ6ccwi9yJmnhciFdOUhihwnxGWwxCFfO5wWCtxPeUEBUpq2kJ6FGFVvR4U3OMkc1U3w3dCVPv5Ch9pYzI)