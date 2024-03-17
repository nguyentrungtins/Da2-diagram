sequenceDiagram
    participant Client
    participant Auth
    participant Route
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Route: Tạo mới tuyến đường
    Route->>+Route: Xử lý yêu cầu tạo mới
    Route-->>-Client: Trả kết quả



[![](https://mermaid.ink/img/pako:eNptUc9KwzAYf5WPXF1fIIeBzNsuoh6G5BLSuIa1yZYmgzF2EJ_AswgOD4IgqDdbZIeK75E38Wtr3XDLJcmP37_kWxJhYkkoyeXMSy3kieJjyzOmAdeUW6eEmnLtYJAqqd0-fuxdso-eGe_kITiVp9JmKs-V0YNEignTLa31j_r9o9qRwqhaC3BJKN8E6PH3ayjvFcTVhx63_JpVsw9YUhiqUN5k4CyHOVe4V-8wrx5g5hehvP5NPKCM0DFq84eh2DgUhOIRJn92_7PxlRQuQrE2kIXyDqMwodho-LptKndtG-aOZBTKF0irT1hUzx5EKJ48uK3Nrqiu1H4OJtmmzrYa06RHMnwEVzFOcVkLGXGJzCQjFI8xtxNGmF4hj3tnzhdaEOqslz3ipzF33cQJveJpjigO6tKY7r76ATuX1JE?type=png)](https://mermaid.live/edit#pako:eNptUc9KwzAYf5WPXF1fIIeBzNsuoh6G5BLSuIa1yZYmgzF2EJ_AswgOD4IgqDdbZIeK75E38Wtr3XDLJcmP37_kWxJhYkkoyeXMSy3kieJjyzOmAdeUW6eEmnLtYJAqqd0-fuxdso-eGe_kITiVp9JmKs-V0YNEignTLa31j_r9o9qRwqhaC3BJKN8E6PH3ayjvFcTVhx63_JpVsw9YUhiqUN5k4CyHOVe4V-8wrx5g5hehvP5NPKCM0DFq84eh2DgUhOIRJn92_7PxlRQuQrE2kIXyDqMwodho-LptKndtG-aOZBTKF0irT1hUzx5EKJ48uK3Nrqiu1H4OJtmmzrYa06RHMnwEVzFOcVkLGXGJzCQjFI8xtxNGmF4hj3tnzhdaEOqslz3ipzF33cQJveJpjigO6tKY7r76ATuX1JE)

