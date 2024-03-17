sequenceDiagram
    Client->>+Server: Thực hiện việc đăng nhập
    Server-->>-Google OAuth2: Redirect đến đăng nhập google
    Google OAuth2-->>Server: Redirect đến đăng nhập google
    Server-->>Client: Redirect trang đăng nhập Google
    Client->>Server: Nhập thông tin đăng nhập
    Server-->>Google OAuth2: Kiểm tra thông tin đăng nhập
    Google OAuth2-->>+Server: Trả thông tin đăng nhập
    Server-->>Server: Kiểm tra người dùng có tồn tại trong database không
    Server-->>Server: Nếu không thì tạo account mới
    Server-->>Server: Nếu có thì trả kết quả đăng nhập thành công
    Server-->>-Client: Trả kết quả từ Server
https://mermaid.ink/img/pako:eNqNkzFLw0AUx7_KcavN4pihIAodhAq2k2Q5L6_J0eSuTe8KUjp1cBZHERRHFRRdTAaHFr_HfRNfksY2VqsZksvx__3f-79LJpQrH6hLRzA0IDkcCBYkLPYkwWs_EiC102zudCAZQ-KSbmizZ05CYbNzScb5g5PFxWImAyJDmz4OSrLUO4g6LaWCCMjRntHhrkuOwRcJcI2UTd9lHSZBIS49amBuVTXxf4tVG2WUNVYnDJk62lpDv7JXVdulRofzVyS0kNtzf4t9iKOaxXnVPxw2Uq9mn9j07t_1K2qtsAw-nmx2LYg_f0OOz1-IttmlxHt6K1CicNdnmp2yEZB-Ueg32zZO3iw1eU8PhYkijHNlpCaxza7EdrioX5BFsD5uajI0-bp-LCi6kSHqf-jHqQ62u2GC2e6XSk_SBo0hiZnw8WOf5C4e1SHE4FEXlz70mIm0Rz05RSkzWnXOJKeuTgw0qBngWKp_g7o9Fo1wd8DkiVLV-_QTTN5VWw?type=png