sequenceDiagram
    participant Client
    participant Auth
    participant Vessel
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Vessel: Cập nhật tàu
    Vessel->>+Vessel: Xử lý yêu cầu cập nhật
    Vessel-->>-Client: Trả kết quả
    
[![](https://mermaid.ink/img/pako:eNptUU1KAzEUvsojW9sLZFGQuutGVKRINiETO6EzmWnmpTCULsRzCBUXglBQd84gLgLeIzcx09hqabPIz5fv5yVvQUSRSEJJJWdWaiHPFJ8YnjMNYZTcoBKq5BphmCmp8RA_tZgeoteyqmR2iF8UmTyXJldVpQo9TKWYMh1pMaA_GJx0lhTG7lEApr59E6An36--fVCQuA89ifyO1bGPWFIYKd_e54CGw5yrsLp3mLsVzGzt27vfxCPKfnDsx_yRb74wCHzzBNOd3X52fCaFoW_WJeg0LAjoVjbS4vV_4ti3a8jcJ9TuxYLwzfNm3on3dF0t8VcoXJlNHX81MU16JA_Vc5WE_i06JSOYylwyQsM24WbKCNPLwOMWi8taC0LRWNkjtkw4bntN6C3PqoCGDt0Uxfa8_AFEvM-r?type=png)](https://mermaid.live/edit#pako:eNptUU1KAzEUvsojW9sLZFGQuutGVKRINiETO6EzmWnmpTCULsRzCBUXglBQd84gLgLeIzcx09hqabPIz5fv5yVvQUSRSEJJJWdWaiHPFJ8YnjMNYZTcoBKq5BphmCmp8RA_tZgeoteyqmR2iF8UmTyXJldVpQo9TKWYMh1pMaA_GJx0lhTG7lEApr59E6An36--fVCQuA89ifyO1bGPWFIYKd_e54CGw5yrsLp3mLsVzGzt27vfxCPKfnDsx_yRb74wCHzzBNOd3X52fCaFoW_WJeg0LAjoVjbS4vV_4ti3a8jcJ9TuxYLwzfNm3on3dF0t8VcoXJlNHX81MU16JA_Vc5WE_i06JSOYylwyQsM24WbKCNPLwOMWi8taC0LRWNkjtkw4bntN6C3PqoCGDt0Uxfa8_AFEvM-r)