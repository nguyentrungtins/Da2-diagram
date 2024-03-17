sequenceDiagram
    participant Client
    participant Auth
    participant Container
    participant RolePermissionCheck

    Client->>+Auth: Xác thực người dùng
    Auth->>+RolePermissionCheck: Kiểm tra vai trò và quyền
    RolePermissionCheck-->>-Auth: Kết quả kiểm tra
    Auth->>+Container: Tìm kiếm container
    Container->>+Container: Xử lý yêu cầu tìm kiếm
    Container-->>-Client: Trả kết quả

[![](https://mermaid.ink/img/pako:eNptkc1KAzEUhV_lkq3tC2RRkLrrRtRFkWxCJnZCJ0mbuSmU0oX4HILiQhAFdecM0kXA98ibmHFsS3-yyd93zrnJXRBhM0koKeXUSyPkmeIjxzUzkMaEO1RCTbhB6BdKGjw8P_WYH6GtQa6MdIdXF7aQ59JpVZbKmn4uxZiZFmszur3eSeNKYRgeBWAe6w8BZvTzHut7BVn4MqOWb6iGPmJJYaBifacBHYcZV2kOnzALDzD181jf_iceUXaTY7fNH8RqhUkQqycYb-x2szcvpXAVXnXDVSsNYvcDNtSeZBjrNyjCN8zDiwcRq2cPuLXZFzeltZ-U0txfWdsSmSEdotNjuMpSRxeNmBHMpZaM0LTMuBszwswycdyjvZwbQSg6LzvETzKO6-4TesOLMp2mhl1bu94vfwFTC9WT?type=png)](https://mermaid.live/edit#pako:eNptkc1KAzEUhV_lkq3tC2RRkLrrRtRFkWxCJnZCJ0mbuSmU0oX4HILiQhAFdecM0kXA98ibmHFsS3-yyd93zrnJXRBhM0koKeXUSyPkmeIjxzUzkMaEO1RCTbhB6BdKGjw8P_WYH6GtQa6MdIdXF7aQ59JpVZbKmn4uxZiZFmszur3eSeNKYRgeBWAe6w8BZvTzHut7BVn4MqOWb6iGPmJJYaBifacBHYcZV2kOnzALDzD181jf_iceUXaTY7fNH8RqhUkQqycYb-x2szcvpXAVXnXDVSsNYvcDNtSeZBjrNyjCN8zDiwcRq2cPuLXZFzeltZ-U0txfWdsSmSEdotNjuMpSRxeNmBHMpZaM0LTMuBszwswycdyjvZwbQSg6LzvETzKO6-4TesOLMp2mhl1bu94vfwFTC9WT)