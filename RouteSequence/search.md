sequenceDiagram
    participant Client
    participant Route
    participant RoutePortManager

    Client->>+Route: Chọn tuyến đường
    Route-->>-Client: Trả tuyến đường đã chọn
    Client->>+RoutePortManager: Tìm kiếm thông tin các cảng trong tuyến đường
    RoutePortManager->>+Route: Truy vấn thông tin các cảng trong tuyến đường
    Route-->>-RoutePortManager: Trả danh sách các cảng
    RoutePortManager-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqdkrFOwzAQhl_l5JXmBTJ0KSsSgk7Ii-WYxEpzTt0zUlT1ERh4AAZUsTEwMKUDQxDvkTfhkqhSpLQd8GDdnf777s6-rdAuMSIWG7MOBrW5tir1qpAIfErlyWpbKiRYrKxBmsbvXCBzJnzrPN0oVKnxEgfNgInm86teEcMiaw_PCBSqtv5G-Hn5_WwPr5gO8l4UsTwaEmNY-rbeT-VsNXvQPexkpVEvDGk-CsgtIwqgrPnifLIIunnToJnf-d5194W2RsTRPEsfKnhq63f8P7kf-ETX_eiJwgw2zMvG1DN9TV8u56oE68C2RDEThfGFsgmvwLZjSEGZKYwUMZuJ8rkUEnesU4HcfYVaxOSDmYlQJoqO6yLiR7XacJT__sG5o7_7A5_a8_U?type=png)](https://mermaid.live/edit#pako:eNqdkrFOwzAQhl_l5JXmBTJ0KSsSgk7Ii-WYxEpzTt0zUlT1ERh4AAZUsTEwMKUDQxDvkTfhkqhSpLQd8GDdnf777s6-rdAuMSIWG7MOBrW5tir1qpAIfErlyWpbKiRYrKxBmsbvXCBzJnzrPN0oVKnxEgfNgInm86teEcMiaw_PCBSqtv5G-Hn5_WwPr5gO8l4UsTwaEmNY-rbeT-VsNXvQPexkpVEvDGk-CsgtIwqgrPnifLIIunnToJnf-d5194W2RsTRPEsfKnhq63f8P7kf-ETX_eiJwgw2zMvG1DN9TV8u56oE68C2RDEThfGFsgmvwLZjSEGZKYwUMZuJ8rkUEnesU4HcfYVaxOSDmYlQJoqO6yLiR7XacJT__sG5o7_7A5_a8_U)