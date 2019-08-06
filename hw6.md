# 使用类图，分别对 Asg_RH 文档中 Make Reservation 用例以及 Payment 用例开展领域建模。然后，根据上述模型，给出建议的数据表以及主要字段，特别是主键和外键。
![](https://github.com/gongwj7/software-analysis-design/blob/master/hw6-1.png?raw=true)

![](https://github.com/gongwj7/software-analysis-design/blob/master/hw6-2.png?raw=true)

Location (ID/Key, Name)

Hotel (ID/Key, LocationID/FKey, Name, Address, Star)

Room (ID/Key, Type, Price, IsAvailable)

Traveler (ID/Key, Name, Email)

Reservation (ID/Key, TravelerID/FKey, HotelID/FKey, Date, Time, CheckInDate, CheckOutDate, AdultNum, ChildNum, ChildAge)

Payment (ID/Key, ReservationID/FKey, Date, Time, Total)

CreditCard (ID/Key, TravelerID/FKey, PaymentID/FKey, Number, SecurityCode, ExpiryDate)
# 使用 UML State Model，对每个订单对象生命周期建模
![](https://github.com/gongwj7/software-analysis-design/blob/master/hw6-3.png?raw=true)
