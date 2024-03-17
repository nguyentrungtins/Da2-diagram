sequenceDiagram
    participant Client
    participant Route
    participant Port
    participant RoutePortManager

    Client->>+Route: Chọn tuyến đường
    Route-->>-Client: Trả tuyến đường đã chọn
    Client->>+Port: Chọn cảng
    Port-->>-Client: Trả cảng đã chọn
    Client->>+RoutePortManager: Cập nhật thông tin cảng trong tuyến đường
    RoutePortManager->>+Route: Cập nhật thông tin cảng trong tuyến đường
    RoutePortManager-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNqtkrFOwzAQQH_F8krzAx66lBUJARPyYjlHYrU5p-55qKp-AgMfwNQZiYEpHRiK-I_8CZdYQVVDO5EhuZzfvctFt5HW5yCVXMEyAlq4dqYIptIo-KpNIGddbZDEbOEAaZy_85FgnL714RzcHd0YNAUEjYlJ8mw6veoJJWZlu39GQXHdNp8ovl6-39v9KxYJ76GM8SwVKvEQ2mY3xjk67ITtZaedus_4bWS5fLB3B3_IE3LJeDod29vmrRZY8oMElYcPFpAb2gkKvrtfGPLIdvx3_lM7nnTOdSSWkWONciIrCJVxOW_JpnNoSSVUoKXiMDdhrqXGLXMmkr9fo5WKQoSJjHVuaNgoqZ7MYsVZXoRH74f37Q9JkQIF?type=png)](https://mermaid.live/edit#pako:eNqtkrFOwzAQQH_F8krzAx66lBUJARPyYjlHYrU5p-55qKp-AgMfwNQZiYEpHRiK-I_8CZdYQVVDO5EhuZzfvctFt5HW5yCVXMEyAlq4dqYIptIo-KpNIGddbZDEbOEAaZy_85FgnL714RzcHd0YNAUEjYlJ8mw6veoJJWZlu39GQXHdNp8ovl6-39v9KxYJ76GM8SwVKvEQ2mY3xjk67ITtZaedus_4bWS5fLB3B3_IE3LJeDod29vmrRZY8oMElYcPFpAb2gkKvrtfGPLIdvx3_lM7nnTOdSSWkWONciIrCJVxOW_JpnNoSSVUoKXiMDdhrqXGLXMmkr9fo5WKQoSJjHVuaNgoqZ7MYsVZXoRH74f37Q9JkQIF)