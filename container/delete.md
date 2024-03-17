sequenceDiagram
    participant Client
    participant Auth
    participant Container
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Container: Xóa container
    Container->>+Container: Xử lý yêu cầu xóa
    Container-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptUc1KAzEQfpUhV7svkENB6q0XUQ8iuQzZuBu6O2mzSbGUHsTnEBQPgiD4c7KLeFjwPfImZl1b6U8uSSbf32TmTJpUMc4qNfGKpDrSmFksBUFcY7ROSz1GcjAotCK3Wz_0Lt-DNuRQk7K7TyemUMfKlrqqtKFBruRIUAfrPJJ-_6BV5XDe3EtweahfJVD2_RLqWw1p80FZh29RLXqPJIehDvVNCc4iTFHHvXmDaXMHEz8L9fWf4x5mEhWTzn8Yll8uEsLyAUZruU3vdadt3HcEudn5-nkbG-pnKJpPmDVPHmRYPnq4ivxtVhum-xYOZ_Y3yH8oQazHyhgfdRpnOG_JgrlclUowHo8p2pFgghYRh96Z0xlJxp31qsf8OEW3mjfjl1hUsRpHdGHM6r74AUkczhs?type=png)](https://mermaid.live/edit#pako:eNptUc1KAzEQfpUhV7svkENB6q0XUQ8iuQzZuBu6O2mzSbGUHsTnEBQPgiD4c7KLeFjwPfImZl1b6U8uSSbf32TmTJpUMc4qNfGKpDrSmFksBUFcY7ROSz1GcjAotCK3Wz_0Lt-DNuRQk7K7TyemUMfKlrqqtKFBruRIUAfrPJJ-_6BV5XDe3EtweahfJVD2_RLqWw1p80FZh29RLXqPJIehDvVNCc4iTFHHvXmDaXMHEz8L9fWf4x5mEhWTzn8Yll8uEsLyAUZruU3vdadt3HcEudn5-nkbG-pnKJpPmDVPHmRYPnq4ivxtVhum-xYOZ_Y3yH8oQazHyhgfdRpnOG_JgrlclUowHo8p2pFgghYRh96Z0xlJxp31qsf8OEW3mjfjl1hUsRpHdGHM6r74AUkczhs)