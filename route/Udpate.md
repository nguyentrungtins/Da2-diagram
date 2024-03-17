sequenceDiagram
    participant Client
    participant Auth
    participant Route
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Route: Cập nhật tuyến đường
    Route->>+Route: Xử lý yêu cầu cập nhật
    Route-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUctKw0AU_ZXLbG1_YBYFqbtuRF0UyWaYjM3QZJJO7hRK6UL8Aj9AUFwIQkHdmSBdRPyP-ZPeJLYWm1nM43DOuefOXTKZhopxlquZU0aqMy0mViSBAVqZsKilzoRBGMZaGTzGTx1Gx-hF6lB1wbE6VzbRea5TM4yUnAampbX-_cHgpHbkMK6eJGDky3cJZvLz5ssHDWH1aSYtv2bV7A5LDiPty7sE0AqYC01n9QHz6hFmbuHL29-KHco-Ofbb-iNfbJAEvniG6d7uf23qksPQF-sMTEQHAlKJYmPg-77JvIvbUA80Y1-uIa6-YFG9OpC-eGn2vc-hqg7Vfg-HK9sE-gvHeiyhJoQOaYrLWhYwjFSiAsbpGgo7DVhgVsQTDtPLhZGMo3Wqx1wWCtxNnPEbEeeE0qCu03T3Xm0BWHzUyQ?type=png)](https://mermaid.live/edit#pako:eNptUctKw0AU_ZXLbG1_YBYFqbtuRF0UyWaYjM3QZJJO7hRK6UL8Aj9AUFwIQkHdmSBdRPyP-ZPeJLYWm1nM43DOuefOXTKZhopxlquZU0aqMy0mViSBAVqZsKilzoRBGMZaGTzGTx1Gx-hF6lB1wbE6VzbRea5TM4yUnAampbX-_cHgpHbkMK6eJGDky3cJZvLz5ssHDWH1aSYtv2bV7A5LDiPty7sE0AqYC01n9QHz6hFmbuHL29-KHco-Ofbb-iNfbJAEvniG6d7uf23qksPQF-sMTEQHAlKJYmPg-77JvIvbUA80Y1-uIa6-YFG9OpC-eGn2vc-hqg7Vfg-HK9sE-gvHeiyhJoQOaYrLWhYwjFSiAsbpGgo7DVhgVsQTDtPLhZGMo3Wqx1wWCtxNnPEbEeeE0qCu03T3Xm0BWHzUyQ)