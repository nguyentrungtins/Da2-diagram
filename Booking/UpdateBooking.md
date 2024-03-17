sequenceDiagram
    participant Client
    participant Auth
    participant Booking
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Booking: Cập nhật booking
    Booking->>+Booking: Xử lý yêu cầu cập nhật
    Booking-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUU9LwzAU_yqPXF2_QA4DrbddRD0M6SWmsQ1tky5NBmXsIH4OQfEgCAP1Zot4KPg98k2Wru10dDnkJS-_P-_lrRCVIUMYFWxhmKDsnJNIkSwQ4FZOlOaU50Ro8FPOhB7nT42Ox9kzKRMuovHDpUzZBVMZLwouhR8zmgSig3UO3nR60mpimDfPFHRs6w8KIvp9t_Ujh7D5GmRbVIs-Iolhxm39kIFWBJaEu9h8wrJ5goUpbX3fOx5hek7R6_xntvrRjmCrF0j2cofefZ8YfFttchCxCxpu_3ffQw7Qc1tvIG2-oWzeDFBbve72vcIhsy2p-xwM12pXzl9paIIy1wLhoZviqiUGSMcsYwHC7hgSlQQoEGuHI0bLq1JQhLUybIJMHhI9TBzhO5IWLuvGdCPlcF9vAXnJ0TE?type=png)](https://mermaid.live/edit#pako:eNptUU9LwzAU_yqPXF2_QA4DrbddRD0M6SWmsQ1tky5NBmXsIH4OQfEgCAP1Zot4KPg98k2Wru10dDnkJS-_P-_lrRCVIUMYFWxhmKDsnJNIkSwQ4FZOlOaU50Ro8FPOhB7nT42Ox9kzKRMuovHDpUzZBVMZLwouhR8zmgSig3UO3nR60mpimDfPFHRs6w8KIvp9t_Ujh7D5GmRbVIs-Iolhxm39kIFWBJaEu9h8wrJ5goUpbX3fOx5hek7R6_xntvrRjmCrF0j2cofefZ8YfFttchCxCxpu_3ffQw7Qc1tvIG2-oWzeDFBbve72vcIhsy2p-xwM12pXzl9paIIy1wLhoZviqiUGSMcsYwHC7hgSlQQoEGuHI0bLq1JQhLUybIJMHhI9TBzhO5IWLuvGdCPlcF9vAXnJ0TE)