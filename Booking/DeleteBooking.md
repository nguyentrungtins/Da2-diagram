sequenceDiagram
    participant Client
    participant Auth
    participant Booking
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Booking: Xóa booking
    Booking->>+Booking: Xử lý yêu cầu xóa
    Booking-->>-Client: Trả kết quả


[![](https://mermaid.ink/img/pako:eNptUU1KxDAUvsojW6cXyGJAx91sRF2IZBPT2Ia2SSdNBsswC_EcguJCEAR_VraIi8LcIzcxta06dLJJ8vL9vbwVYirkCKOCLyyXjB8KGmmaEQl-5VQbwUROpYFZKrg04_q-NfG4eqBUImQ0fjhWKT_iOhNFIZScxZwlRHawziGYTvdaTQxnzT0DE7v6lYGMNi-uvhUQNh-DbItq0TskMcyFq28yMJrCkgq_N2-wbO5gYUtXX_eOO5iBVww6_7mrvownuOoBkl-5be--zzbsO4WL_133T9soVz9D2nxC2TxZYK56tHDlmduMNkL3GRhO9Y_9XxQi0QRlPjQVoZ_bqqUSZGKecYKwP4ZUJwQRufY4ao06KSVD2GjLJ8jmITXDjBG-pGnhq34w50oN9_U3P6TI_w?type=png)](https://mermaid.live/edit#pako:eNptUU1KxDAUvsojW6cXyGJAx91sRF2IZBPT2Ia2SSdNBsswC_EcguJCEAR_VraIi8LcIzcxta06dLJJ8vL9vbwVYirkCKOCLyyXjB8KGmmaEQl-5VQbwUROpYFZKrg04_q-NfG4eqBUImQ0fjhWKT_iOhNFIZScxZwlRHawziGYTvdaTQxnzT0DE7v6lYGMNi-uvhUQNh-DbItq0TskMcyFq28yMJrCkgq_N2-wbO5gYUtXX_eOO5iBVww6_7mrvownuOoBkl-5be--zzbsO4WL_133T9soVz9D2nxC2TxZYK56tHDlmduMNkL3GRhO9Y_9XxQi0QRlPjQVoZ_bqqUSZGKecYKwP4ZUJwQRufY4ao06KSVD2GjLJ8jmITXDjBG-pGnhq34w50oN9_U3P6TI_w)