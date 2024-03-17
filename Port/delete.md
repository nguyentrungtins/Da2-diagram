sequenceDiagram
    participant Client
    participant Auth
    participant Port
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Port: Xóa cảng
    Port->>+Port: Xử lý yêu cầu xóa
    Port-->>-Client: Trả kết quả

    
[![](https://mermaid.ink/img/pako:eNptkc1KAzEUhV_lkq2dF8iiIHXXTVEXItmETJwJM5NMM0lxKF2IzyEoLgRB8GdlB3ER8D3yJk0cRyttNkluvnPODXeJmEo5wqjhc8sl40eCZppWREJYNdVGMFFTaWBSCi7Nbv3Qmny3OlN6D3usSj7juhJNI5Sc5JwVRPZYb5-MxwfREMOZu2Ngct-9MJDZ17PvbgSk7l1mPR-pSO-xxDAVvruuwGgKCyrC7l5h4W5hblvfXf0k7lEmwTHp86d-_WmCwK_vofi1-58dPxk7faPAAje0Fstbz757gtJ9QOsebeQeLFwGyRYbU_v_YzjV34l_6USiEapCn1SkYU7LqCPI5LziBOFwTKkuCCJyFThqjTppJUPYaMtHyNYpNcNMEb6gZROqYRbnSg331QaHPMPY?type=png)](https://mermaid.live/edit#pako:eNptkc1KAzEUhV_lkq2dF8iiIHXXTVEXItmETJwJM5NMM0lxKF2IzyEoLgRB8GdlB3ER8D3yJk0cRyttNkluvnPODXeJmEo5wqjhc8sl40eCZppWREJYNdVGMFFTaWBSCi7Nbv3Qmny3OlN6D3usSj7juhJNI5Sc5JwVRPZYb5-MxwfREMOZu2Ngct-9MJDZ17PvbgSk7l1mPR-pSO-xxDAVvruuwGgKCyrC7l5h4W5hblvfXf0k7lEmwTHp86d-_WmCwK_vofi1-58dPxk7faPAAje0Fstbz757gtJ9QOsebeQeLFwGyRYbU_v_YzjV34l_6USiEapCn1SkYU7LqCPI5LziBOFwTKkuCCJyFThqjTppJUPYaMtHyNYpNcNMEb6gZROqYRbnSg331QaHPMPY)