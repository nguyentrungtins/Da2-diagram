sequenceDiagram
    participant Client
    participant Auth
    participant User
    participant Role
    participant Permission
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+User: Tìm kiếm thông tin người dùng
    User->>+User: Xử lý yêu cầu tìm kiếm thông tin người dùng
    Auth->>+Role: Tìm kiếm vai trò của người dùng
    Role->>+Role: Xử lý yêu cầu tìm kiếm vai trò
    Auth->>+Permission: Tìm kiếm quyền của người dùng
    Permission->>+Permission: Xử lý yêu cầu tìm kiếm quyền
    Auth->>+RolePermissionCheck: Kiểm tra quyền và vai trò của người dùng
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    User-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqNk09LwzAYxr_KS65uXyCHgczbLuIfGNJLSGMb1qZdmgzG2EH8HILiYSAKKl5cEQ8Bv0e-iYldrVuHW0_t2-f3vE_eJDNEs5AhjAo21kxQdsRJJEkaCHBPTqTilOdEKOgnnAnVrh9qFber5wWT7epJlrB29ZjJlBcFz8R2ovnfjxkdBStZFajb6x34CBiG5o6Cim35QkFEX8-2vOEQmncRVXqv8mofDcOZeUxhxO3yM3WQeRMRKC62gh5owKEtnyAxHzA1DxqoXS40qP3N6hR-YespJoSDkubVeZYLshX2UAPvSlIbrjduprnefqyntrwS_3RvyE2fXUlW3u0JbGwthgG35bUboiS_gSbmdt_ZbNh1XZtudTgGLodylnZ570OtevzZXy-tTpQbi_yRNUggUAelzpzw0N2VmecCpGKWsgBh9xoSOQpQIOZOR7TKTqeCIqykZh2k85Co-l4hfEmSwlXd6b7Isvp7_g3OsW6s?type=png)](https://mermaid.live/edit#pako:eNqNk09LwzAYxr_KS65uXyCHgczbLuIfGNJLSGMb1qZdmgzG2EH8HILiYSAKKl5cEQ8Bv0e-iYldrVuHW0_t2-f3vE_eJDNEs5AhjAo21kxQdsRJJEkaCHBPTqTilOdEKOgnnAnVrh9qFber5wWT7epJlrB29ZjJlBcFz8R2ovnfjxkdBStZFajb6x34CBiG5o6Cim35QkFEX8-2vOEQmncRVXqv8mofDcOZeUxhxO3yM3WQeRMRKC62gh5owKEtnyAxHzA1DxqoXS40qP3N6hR-YespJoSDkubVeZYLshX2UAPvSlIbrjduprnefqyntrwS_3RvyE2fXUlW3u0JbGwthgG35bUboiS_gSbmdt_ZbNh1XZtudTgGLodylnZ570OtevzZXy-tTpQbi_yRNUggUAelzpzw0N2VmecCpGKWsgBh9xoSOQpQIOZOR7TKTqeCIqykZh2k85Co-l4hfEmSwlXd6b7Isvp7_g3OsW6s)