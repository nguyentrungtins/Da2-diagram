sequenceDiagram
    participant Client
    participant Route
    participant Port
    participant RoutePortManager

    Client->>+Route: Chọn tuyến đường
    Route-->>-Client: Trả tuyến đường đã chọn
    Client->>+Port: Chọn cảng
    Port-->>-Client: Trả cảng đã chọn
    Client->>+RoutePortManager: Thêm cảng vào tuyến đường
    RoutePortManager->>+Route: Cập nhật thông tin cảng trong tuyến đường
    RoutePortManager-->>-Client: Trả kết quả


[![](https://mermaid.ink/img/pako:eNqNkrFOwzAQhl_F8krzAh66lBUJARPycnJMYrU5p-4Zqar6CAw8ABJSNyQkBqZ0YAjiPfImXBIFVQ1UeLDP5-__7bO9kcanViq5ssto0dhzB1mAQqPgVkIgZ1wJSGK2cBZpnL_ykew4fenDX3C7dAEImQ0ae6Y3T6bTs45QYpY3-wcUFNdN9YHi8_Hrrdk_YdbjHZQwnvRCJW5CU-3GOEf1TpjO7Hin9hg_GxmWD-7twi_mPXLK8bg6Vub1SzEo7-tnf7KiA-nhVTTVaykw54EE5fU7W5Ebjiwo-Lb_p-24rDnrSCwjxxrlRBY2FOBS_hKb1kNLym1htVQcphDmWmrcMgeR_PUajVQUop3IWKZAw_eR6g4WK87yq996P8y332yc-Uo?type=png)](https://mermaid.live/edit#pako:eNqNkrFOwzAQhl_F8krzAh66lBUJARPycnJMYrU5p-4Zqar6CAw8ABJSNyQkBqZ0YAjiPfImXBIFVQ1UeLDP5-__7bO9kcanViq5ssto0dhzB1mAQqPgVkIgZ1wJSGK2cBZpnL_ykew4fenDX3C7dAEImQ0ae6Y3T6bTs45QYpY3-wcUFNdN9YHi8_Hrrdk_YdbjHZQwnvRCJW5CU-3GOEf1TpjO7Hin9hg_GxmWD-7twi_mPXLK8bg6Vub1SzEo7-tnf7KiA-nhVTTVaykw54EE5fU7W5Ebjiwo-Lb_p-24rDnrSCwjxxrlRBY2FOBS_hKb1kNLym1htVQcphDmWmrcMgeR_PUajVQUop3IWKZAw_eR6g4WK87yq996P8y332yc-Uo)