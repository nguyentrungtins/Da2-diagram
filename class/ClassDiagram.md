classDiagram
    class Route {
        + create()
        + update()
        + delete()
        + search()
    }
    class Port {
        + create()
        + update()
        + delete()
        + search()
    }
    class Vessel {
        + create()
        + update()
        + delete()
        + search()
    }
    class Booking {
        + create()
        + update()
        + delete()
        + search()
    }
    class Container {
        + create()
        + update()
        + delete()
        + search()
    }
    class Auth {
        + googleAuth()
        + credentialAuth()
    }
    class Tracking {
        + containerTracking()
        + vesselTracking()
        + bookingTracking()
    }

    Route --|> Booking : includes
    Port --|> Booking : includes
    Vessel --|> Booking : includes
    Vessel --|> Container : carries
    Booking --|> Container : contains
    Booking --> Auth : requires authentication
    Booking --> Tracking : requires tracking


[![](https://mermaid.ink/img/pako:eNq9k0FuwyAQRa-CZtWo8QVYRGrVA1Rt1EXlzRSmNgpmIsCRqtR3LzF2ZSfO1qzwf-h_9D2cQbEmkKAshvBisPLYlE6k1SvijdtI4pyly3oUyhNGethMtfaobzRNlq61QOhVPWrdNOmVfVwl6INCILtK1DPzwbhqlaynNtbzoIq5snTR5ybpAppcNGinbGa296gWbs4uonHkRzz3PfXFLrOv3MQ1TKF5k-esKH53eRCkqDHcoOHXLcOx7Antre7BweweHqWi2OVupXBEeoH-lzWcgC005Bs0Oj2svsASYk0NlSDTVqM_lFC6Lp3DNvL7j1Mgo29pC3kOhncI8httSOoR3Sfz-N39AZ_kEFg?type=png)](https://mermaid.live/edit#pako:eNq9k0FuwyAQRa-CZtWo8QVYRGrVA1Rt1EXlzRSmNgpmIsCRqtR3LzF2ZSfO1qzwf-h_9D2cQbEmkKAshvBisPLYlE6k1SvijdtI4pyly3oUyhNGethMtfaobzRNlq61QOhVPWrdNOmVfVwl6INCILtK1DPzwbhqlaynNtbzoIq5snTR5ybpAppcNGinbGa296gWbs4uonHkRzz3PfXFLrOv3MQ1TKF5k-esKH53eRCkqDHcoOHXLcOx7Antre7BweweHqWi2OVupXBEeoH-lzWcgC005Bs0Oj2svsASYk0NlSDTVqM_lFC6Lp3DNvL7j1Mgo29pC3kOhncI8httSOoR3Sfz-N39AZ_kEFg)