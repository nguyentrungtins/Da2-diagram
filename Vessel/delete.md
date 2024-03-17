sequenceDiagram
    participant Client
    participant Auth
    participant Vessel
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Vessel: Xóa tàu
    Vessel->>+Vessel: Xử lý yêu cầu xóa
    Vessel-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNptUU1KAzEUvsojW9sLZFGQuutGVEQkm5B5dkJnMtNMUiylC_EcQsWFIAj-rJxBXAS8R27SjLHKMM0meV--n5e8FRFFgoSSCucWlcAjyaea50xBWCXXRgpZcmVgnElUpo8fWpP20XOsKsz6-EmR4THqXFaVLNQ4RTFjKtJiwHA0OmgtKVy4ewEm9c2rADX9fvHNnYTEfahp5Leslr3HksJE-uY2B6M5LLgMu3uDhdvA3C59c_ObuEc5DI7DmD_x9ZcJAl8_wOzPrpsdn9n2-s7BuI2N1xHuEHzzDJn7hKV7siB8_WjhOog6_DY7_gKFM_2T-98DU2RA8tAtl0mY16pVMmJSzJERGo4J1zNGmFoHHremOF0qQajRFgfElgk3u9kSesWzKqBhIpdFsavXW5Dlxq8?type=png)](https://mermaid.live/edit#pako:eNptUU1KAzEUvsojW9sLZFGQuutGVEQkm5B5dkJnMtNMUiylC_EcQsWFIAj-rJxBXAS8R27SjLHKMM0meV--n5e8FRFFgoSSCucWlcAjyaea50xBWCXXRgpZcmVgnElUpo8fWpP20XOsKsz6-EmR4THqXFaVLNQ4RTFjKtJiwHA0OmgtKVy4ewEm9c2rADX9fvHNnYTEfahp5Leslr3HksJE-uY2B6M5LLgMu3uDhdvA3C59c_ObuEc5DI7DmD_x9ZcJAl8_wOzPrpsdn9n2-s7BuI2N1xHuEHzzDJn7hKV7siB8_WjhOog6_DY7_gKFM_2T-98DU2RA8tAtl0mY16pVMmJSzJERGo4J1zNGmFoHHremOF0qQajRFgfElgk3u9kSesWzKqBhIpdFsavXW5Dlxq8)