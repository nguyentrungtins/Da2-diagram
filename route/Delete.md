sequenceDiagram
    participant Client
    participant Auth
    participant Route
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Route: Tìm kiếm tuyến đường
    Route->>+Route: Xử lý yêu cầu tìm kiếm
    Route-->>-Client: Trả kết quả
[![](https://mermaid.ink/img/pako:eNptUU1KAzEUvsojW9sLZCFI3XUj6qJINiETO6EzmTbzUiilC_EEHkBQXAiioO6cQbqIeI_cxDcda4ttNkk-vr_kzZkqEs04K_XEa6v0sZFDJ3NhgdZYOjTKjKVF6GVGW9zFjzymu-hp4VHvgzN9ol1uytIUtpdqNRK2pbX-3cPDg8aRwyDcK8A01m8K7PD7Nda3BpLwYYctv2E17D2WHPom1tc5oJMwlYb28A7TcAcTP4v11W_iHmWXHLttfj9WSyRBrB5g9Gf3P5teyeE8POcNp1oShxKqpYWvm1XlddsVc0syiPULZOETZuHJg4rVowfc2GyLmkrt51CSW9XZVBOWdVhOj5AmoSnOG6FgmOpcC8bpmEg3EkzYBfGkx-JsZhXj6LzuMD9OJK4nzvilzEpCaVAXRbG-L34A2_PUDw?type=png)](https://mermaid.live/edit#pako:eNptUU1KAzEUvsojW9sLZCFI3XUj6qJINiETO6EzmTbzUiilC_EEHkBQXAiioO6cQbqIeI_cxDcda4ttNkk-vr_kzZkqEs04K_XEa6v0sZFDJ3NhgdZYOjTKjKVF6GVGW9zFjzymu-hp4VHvgzN9ol1uytIUtpdqNRK2pbX-3cPDg8aRwyDcK8A01m8K7PD7Nda3BpLwYYctv2E17D2WHPom1tc5oJMwlYb28A7TcAcTP4v11W_iHmWXHLttfj9WSyRBrB5g9Gf3P5teyeE8POcNp1oShxKqpYWvm1XlddsVc0syiPULZOETZuHJg4rVowfc2GyLmkrt51CSW9XZVBOWdVhOj5AmoSnOG6FgmOpcC8bpmEg3EkzYBfGkx-JsZhXj6LzuMD9OJK4nzvilzEpCaVAXRbG-L34A2_PUDw)