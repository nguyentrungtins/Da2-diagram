sequenceDiagram
    participant Client
    participant Auth
    participant Port
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Port: Tìm kiếm cảng
    Port->>+Port: Xử lý yêu cầu tìm kiếm
    Port-->>-Client: Trả kết quả


[![](https://mermaid.ink/img/pako:eNptkUFKAzEUhq_yyNb2AlkUpO66KeqiSDYhEzuhk2SaSQpD6UI8h6C4EERB3dlBugh4j9zExHEcpc0myZvv__-XeWvEdMYRRhVfOq4YPxF0bqgkCuIqqbGCiZIqC-NCcGX368fO5vvVqTYH2FNd8Ck3UlSV0Gqcc7YgqsVa--FodJQMMcz8HQObh-aVgZp_voTmRkDm39W85ROV6AOWGCYiNNcSrKGwoiLu_g1W_haWrg7N1U_iAeUwOg7b_EnY7mwUhO09LH7t_menR2I4908yIdudBBbxrsP0tadmoXmGwn9A7R9d4h4c2F75R5J6aP9G9Dbf-X0vRKEBkrFrKrI4tXXSEWRzLjlBOB4zahYEEbWJHHVWn9WKIWyN4wPkyozabsIIX9KiitU4mQutu_vmC-Vxy1A?type=png)](https://mermaid.live/edit#pako:eNptkUFKAzEUhq_yyNb2AlkUpO66KeqiSDYhEzuhk2SaSQpD6UI8h6C4EERB3dlBugh4j9zExHEcpc0myZvv__-XeWvEdMYRRhVfOq4YPxF0bqgkCuIqqbGCiZIqC-NCcGX368fO5vvVqTYH2FNd8Ck3UlSV0Gqcc7YgqsVa--FodJQMMcz8HQObh-aVgZp_voTmRkDm39W85ROV6AOWGCYiNNcSrKGwoiLu_g1W_haWrg7N1U_iAeUwOg7b_EnY7mwUhO09LH7t_menR2I4908yIdudBBbxrsP0tadmoXmGwn9A7R9d4h4c2F75R5J6aP9G9Dbf-X0vRKEBkrFrKrI4tXXSEWRzLjlBOB4zahYEEbWJHHVWn9WKIWyN4wPkyozabsIIX9KiitU4mQutu_vmC-Vxy1A)