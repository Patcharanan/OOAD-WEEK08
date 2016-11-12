#นายพชรนันท์ จันทร์รักษ์ 57030198
## ส่งงาน Use case Diagram 5 ข้อ
* รูปที่ 1 Cinema
```
@startuml
title Hospital 
:customer: -> (Check seat)
:customer: --> (Reserve seat)
:customer: --> (Payment)
(Reserve seat) <--- :Officer: : Check
:Officer: -> (Payment) : receive money
(Payment) .. (Cash)
(Payment) .. (Card)
@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TO_12eCm44Jl-nLxQpt43mYb27v0I_yWn153JOHaBVZtNNjHaLxdpUpCDaLSbZcE9456S1iIecEoVYuoHMJBvixNTe1_Su6Jwe1Mza91_k0FVReb8YcWev5lnXYsZxuFVZLR_dNGfkpJYZCyWgRZbB3GHkfQvxaoL2SjTzfAbzt5qroc1gdJzxy0)

* รูปที่ 2 Hospital
```
@startuml
left to right direction
title Hospital 
:patient: -> (appointment)
:patient: -> (cancle)
:patient: --> (cure)
:patient: --> (Pay)
(appointment) <-- :Staff: : Check
(cancle) <-- :Staff:
(cure) <-- :Doctor:
(Pay) <-- :Clerk:
@enduml

```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/PP1DRW8n34RtFeLtC8lX016gaAQBxbgr9x0oJiSYaumSKudR4neX6F3oVTRppw4OgPtc2963eMLK-PqCHr7s9Zc1YKN6ZrmMCOe8RY4JJkQmVyCjBKkMP7C5tLFaAVd8A_gFJ_eAl-ZS0QnikEzxT3z68JXqE4piZt2JFeRGb0szPszPAxiQ6neYwz51gutx344yQzknThLX3kkzB7-CSqvyXiqzskrmEr2PkbUeOxSoNfNVN5Yhfp3LFZXm6kjxBm00)

* รูปที่ 3 ลงทะเบียน
```
@startuml
title enroll in 
left to right direction
skinparam packageStyle rect
actor Student
actor RegistrationOfficer
actor Clerk
rectangle checkout {
  Student -- (Register)
  (Register) --> (Check the course)
  Student -- (Payment information)
  Clerk -- (Payment information)
  RegistrationOfficer - (Register)
  RegistrationOfficer - (Check the course)
}
@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/VP5DZi8m38NtEOLta0KSe8iH4WS0mGcir6sjvWSvxaZLYBkJC4LeO6QoYkttFZybkwmeEWLlbDKJK9JaFN04uwbJq0J2_Q3Gif1JJj7aaUC51GDSq8tOqrddugnZWqwJm5cdbkAZEb7FMGMh-T1rx4YMoTwJZAOQCVO5uGPoOveKlWmy8B3PmFeRGM9B_rcKqGUizzK4EXHxcYIJVV4USGxrph5B4kufgkI--p_1Bx7X9SeValT4LxESLRFe6gZPbzKMclfyn9y48KMQpUevscuB4VDWtvlIsX_4YZnH9YcSJ5XqPaUnBRzx0m00)

* รูปที่ 4 Check Out
```
@startuml
title Check out
left to right direction
skinparam packageStyle rect
actor Thetenants
actor Officer
rectangle Checkout {
    Thetenants -- (Check out)
    (Check out) --> (Check the room)
    (Refund guarantee) ..> (Check the room)
    (Check the room) -- Officer
    Thetenants -- (Pay)
    (Pay) -- Officer
}
@enduml

```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TP5DReGm38NtFeLtbCLm01QZaNg0LjDUm0g6H80pIambLFNkurJGcVvb5Viz-trAJbafwJ9Fe44dnaVFRiIuA4pSAsh450Qls8N4JaCKo6EG2oMQyK9kf85VTBN18WCvZGbVFIiBYUQjyTJtmN62uY4PzXXBmNT0ExS9F1pmuGkY_bJlQfEFUwtUKcESDzEP-qKw71PZ4sMkiMd-y_vebj2TyG-SPrgtkNAxDty0GDLkLOk5pImpYv6svKaul37EKNY5wYOrZI5GzlNlPkhgRnlBoZDdJhOdCvaFgXDBPpzs1G00)

* รูปที่ 5 Online Shop
```
@startuml
title OnlineShop
left to right direction
skinparam packageStyle rect
actor customer
actor merchant
rectangle OnlineShop {
    customer -- (OnlineStore) : Open
    customer -- (Add to Cart) : Oder
    customer -- (Pay) 
    (Pay) . (Cash)
    (Pay) . (card)
    (Pay) -right- merchant : check
    merchant -right- (Delive) : sent
    (Delive) -- customer : recive
    (OnlineStore) -- merchant : check 
}
@enduml
```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/RL91ReCm4BplA_OME3WFu52bIkzKpGiiUm4Bi97jj49L_zwr2JI8-hIUdPsTiNm9KVfu7mU89Ww4jHsCfLld9XYeYHWTUjDs4RNnfA9n5a9lx2Iz776IgfSjtUBCawaDKaNdKTr3T2FvnvKhrKaR8L6aRNThy1kGppg2Gc3nwF8ibLXXFP4zabwrJkwkR3-JDEyxaDxbN6A6b_ACnLM6hjn3Idhz38aSMMp6MLvrfFfCsS2LLRpHO3wpqq2SCkki69lO35NfZHXT6BkGuhWCuGS0JbNTD4QHhr2yP7iZxoWNBM8n79sb6Kv_hRDsNtOB-cyZnNrMJj8V5CYpNY39NBYGrVmjVW40)

#นายพชรนันท์ จันทร์รักษ์ 57030198
