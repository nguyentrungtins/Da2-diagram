sequenceDiagram
    participant Client
    participant Auth
    participant Vessel
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Vessel: Tìm kiếm tàu
    Vessel->>+Vessel: Xử lý yêu cầu tìm kiếm
    Vessel-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNptkcFKAzEQhl9lyNXuC-RQkHrrRVSkSC4hG7uhu9ltNimU0oP4HELFgyAK6s1dpIeA75E3cdbYamlzSfLv9_8z2VkQUaaSUFLLqZNayBPFx4YXTAOuihurhKq4tjDIldR2Xz92NttXL2Vdy3xfPytzeSpNoepalXqQSTFhOmKxQNLvH3WRFEb-XoDNQvsmQI-_XkN7pyD1H3oc-Y7q6AORFIYqtLcFWMNhxhXu_h1mfgVTNw_tzW_FA84EE5NYfxiatUVDaB5gso3brR2fSeHCPxcd1KwR8isXqfj1PzcK7Qvk_hPm_smBCM2jQ37r3bF1ncR_gvnmp4u_jpgmPVJg71ylOL1F52TEZrKQjFA8ptxMGGF6iRx3tjyfa0GoNU72iKtSbjeTJvSa5zWqOJ-rstzcl98fDc4n?type=png)](https://mermaid.live/edit#pako:eNptkcFKAzEQhl9lyNXuC-RQkHrrRVSkSC4hG7uhu9ltNimU0oP4HELFgyAK6s1dpIeA75E3cdbYamlzSfLv9_8z2VkQUaaSUFLLqZNayBPFx4YXTAOuihurhKq4tjDIldR2Xz92NttXL2Vdy3xfPytzeSpNoepalXqQSTFhOmKxQNLvH3WRFEb-XoDNQvsmQI-_XkN7pyD1H3oc-Y7q6AORFIYqtLcFWMNhxhXu_h1mfgVTNw_tzW_FA84EE5NYfxiatUVDaB5gso3brR2fSeHCPxcd1KwR8isXqfj1PzcK7Qvk_hPm_smBCM2jQ37r3bF1ncR_gvnmp4u_jpgmPVJg71ylOL1F52TEZrKQjFA8ptxMGGF6iRx3tjyfa0GoNU72iKtSbjeTJvSa5zWqOJ-rstzcl98fDc4n)