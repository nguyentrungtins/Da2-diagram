sequenceDiagram
    participant Client
    participant Auth
    participant User
    participant Role
    participant Permission
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+User: Xóa người dùng
    User->>+User: Xử lý yêu cầu xóa người dùng
    Auth->>+Role: Xóa vai trò của người dùng
    Role->>+Role: Xử lý yêu cầu xóa vai trò
    Auth->>+Permission: Xóa quyền của người dùng
    Permission->>+Permission: Xử lý yêu cầu xóa quyền
    Auth->>+RolePermissionCheck: Kiểm tra quyền và vai trò của người dùng
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    User-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqNU89KwzAYf5WPXF1fIIeBzNsu4h8QySWkcQ1r0y1NhmXsID6HoHgYCIJ_Tq6Ih4LvkTcxsa2d6yb2lH75_Uu-L3PE0pAjjDI-NVwyfiDoSNGESHDfhCotmJhQqWEQCy51t75vdNStnmZcdatHacy71UOuEpFlIpXbGe3-IOJsTGpYFSjo9_d8BAxn5R0DHdnimYEcfT7Z4kZAWL7JUYX3KI_20Tz6lW6F-e01mC0eIS7fIS8fDDC7Whq43EVtHHzo2mFGBWhVvjhqsdzO8ug11i7DRum3VXs3teHU5La4kn_4tZSOwC7vWrR7yo3WYBgKW1wnLmibZFbe_vcaNuQCZxNUzR3a1Yd2knZ1D-Mfj7WOeWg1ERhO1DespRCJeihx4lSEbtbnnkeQjnjCCcJuGVI1JojIhcNRo9PjXDKEtTK8h8wkpLp5Fwhf0DhzVTed52na_C--AA_oTt4?type=png)](https://mermaid.live/edit#pako:eNqNU89KwzAYf5WPXF1fIIeBzNsu4h8QySWkcQ1r0y1NhmXsID6HoHgYCIJ_Tq6Ih4LvkTcxsa2d6yb2lH75_Uu-L3PE0pAjjDI-NVwyfiDoSNGESHDfhCotmJhQqWEQCy51t75vdNStnmZcdatHacy71UOuEpFlIpXbGe3-IOJsTGpYFSjo9_d8BAxn5R0DHdnimYEcfT7Z4kZAWL7JUYX3KI_20Tz6lW6F-e01mC0eIS7fIS8fDDC7Whq43EVtHHzo2mFGBWhVvjhqsdzO8ug11i7DRum3VXs3teHU5La4kn_4tZSOwC7vWrR7yo3WYBgKW1wnLmibZFbe_vcaNuQCZxNUzR3a1Yd2knZ1D-Mfj7WOeWg1ERhO1DespRCJeihx4lSEbtbnnkeQjnjCCcJuGVI1JojIhcNRo9PjXDKEtTK8h8wkpLp5Fwhf0DhzVTed52na_C--AA_oTt4)