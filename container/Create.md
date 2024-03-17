sequenceDiagram
    participant Client
    participant Auth
    participant Container
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Container: Tạo mới container
    Container->>+Container: Xử lý yêu cầu tạo mới
    Container-->>-Client: Trả kết quả


[![](https://mermaid.ink/img/pako:eNptUc1KAzEQfpUhV9sXyKEg9daLqIciuYRs7IbuTtrspFBKD-JjiGDxIAiCenMX8bDge-RNzLq2pT-5JDP5fuZnwZRNNOOs0FOvUekzI0dO5gIhnol0ZJSZSCToZ0YjHeZPPaVH0BZJGtTu8OvCZvpcu9wUhbHYT7UaC2xhrUe31ztpVDkM65UCSkP1rgBHP2-hejCQ1J84avENqkEfkeQwMKG6y4GchJk08a4_YFY_wtTPQ3X773iE2Y2K3dZ_EMpvioRQPsF4I7frvemUw1UoVxbyUN0bULsD2KD2KMNQvUJWf8G8fvGgQvnsgbYy--SmtHZI0c39lbUtUSDrsDw2I00SN7poyIJRqnMtGI_PRLqxYAKXESc92cs5KsbJed1hfpJIWm-f8RuZFTEbF3Zt7Tpe_gK0qNYV?type=png)](https://mermaid.live/edit#pako:eNptUc1KAzEQfpUhV9sXyKEg9daLqIciuYRs7IbuTtrspFBKD-JjiGDxIAiCenMX8bDge-RNzLq2pT-5JDP5fuZnwZRNNOOs0FOvUekzI0dO5gIhnol0ZJSZSCToZ0YjHeZPPaVH0BZJGtTu8OvCZvpcu9wUhbHYT7UaC2xhrUe31ztpVDkM65UCSkP1rgBHP2-hejCQ1J84avENqkEfkeQwMKG6y4GchJk08a4_YFY_wtTPQ3X773iE2Y2K3dZ_EMpvioRQPsF4I7frvemUw1UoVxbyUN0bULsD2KD2KMNQvUJWf8G8fvGgQvnsgbYy--SmtHZI0c39lbUtUSDrsDw2I00SN7poyIJRqnMtGI_PRLqxYAKXESc92cs5KsbJed1hfpJIWm-f8RuZFTEbF3Zt7Tpe_gK0qNYV)