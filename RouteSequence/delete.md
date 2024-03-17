sequenceDiagram
    participant Client
    participant Route
    participant Port
    participant RoutePortManager

    Client->>+Route: Chọn tuyến đường
    Route-->>-Client: Trả tuyến đường đã chọn
    Client->>+Port: Chọn cảng cần xóa
    Port-->>-Client: Trả cảng đã chọn
    Client->>+RoutePortManager: Xóa cảng khỏi tuyến đường
    RoutePortManager->>+Route: Xóa thông tin cảng khỏi tuyến đường
    RoutePortManager-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNqdkrFOwzAQhl_F8krzAh66lBUJAQNCXk6OSaw059Q9S1RVHwEhHoCpAysSTO3AEMR75E24JBRVDXTAi8_n7__PZ3spjU-tVHJuZ9GisacOsgClRsGjgkDOuAqQxGTqLNIwf-Ej2WH63Ie_4HbrDBAyGzT2TG-ejMcnHaHEJG-29ygoLprNO4qPx8-XZvuEWY93UMJ40guVuArNZj3EOarXwnRmh5XaY_wUMixnnKdnFHf1K_R0y_xS55s-Yn7YqBLXbLoTFqx5cEe729PuXUtnQnn9xibk8J9-w4YK1pGYRY7lSJY2lOBS_hXL1kFLym1ptVQcphAKLTWumINI_nKBRioK0Y5krFKg3Q-S6hamc87yw994v1uvvgDRxvuZ?type=png)](https://mermaid.live/edit#pako:eNqdkrFOwzAQhl_F8krzAh66lBUJAQNCXk6OSaw059Q9S1RVHwEhHoCpAysSTO3AEMR75E24JBRVDXTAi8_n7__PZ3spjU-tVHJuZ9GisacOsgClRsGjgkDOuAqQxGTqLNIwf-Ej2WH63Ie_4HbrDBAyGzT2TG-ejMcnHaHEJG-29ygoLprNO4qPx8-XZvuEWY93UMJ40guVuArNZj3EOarXwnRmh5XaY_wUMixnnKdnFHf1K_R0y_xS55s-Yn7YqBLXbLoTFqx5cEe729PuXUtnQnn9xibk8J9-w4YK1pGYRY7lSJY2lOBS_hXL1kFLym1ptVQcphAKLTWumINI_nKBRioK0Y5krFKg3Q-S6hamc87yw994v1uvvgDRxvuZ)