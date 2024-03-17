sequenceDiagram
    participant Client
    participant Booking
    participant Route
    participant Port
    participant Vessel

    Client->>+Booking: Tạo booking
    Booking->>+Route: Chọn route
    Route-->>-Booking: Trả route đã chọn
    Booking->>+Port: Chọn port
    Port-->>-Booking: Trả port đã chọn
    Booking->>+Vessel: Chọn vessel
    Vessel-->>-Booking: Trả vessel đã chọn
    Booking->>+Booking: Chọn container(type)
    Booking->>+Booking: Tạo booking
    Booking-->>-Client: Trả kết quả

