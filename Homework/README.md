## ส่งงาน Use case Diagram 5 ข้อ
* รูปที่ 1 Cinema
```

```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TO_12eCm44Jl-nLxQpt43mYb27v0I_yWn153JOHaBVZtNNjHaLxdpUpCDaLSbZcE9456S1iIecEoVYuoHMJBvixNTe1_Su6Jwe1Mza91_k0FVReb8YcWev5lnXYsZxuFVZLR_dNGfkpJYZCyWgRZbB3GHkfQvxaoL2SjTzfAbzt5qroc1gdJzxy0)

* รูปที่ 2 Hospital
```

```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/PP1DRW8n34RtFeLtC8lX016gaAQBxbgr9x0oJiSYaumSKudR4neX6F3oVTRppw4OgPtc2963eMLK-PqCHr7s9Zc1YKN6ZrmMCOe8RY4JJkQmVyCjBKkMP7C5tLFaAVd8A_gFJ_eAl-ZS0QnikEzxT3z68JXqE4piZt2JFeRGb0szPszPAxiQ6neYwz51gutx344yQzknThLX3kkzB7-CSqvyXiqzskrmEr2PkbUeOxSoNfNVN5Yhfp3LFZXm6kjxBm00)

* รูปที่ 3 ลงทะเบียน
```

```
[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/TL7DRi8m3BxdANo37E01UfYGU81Dy0HMwhPMyuCS5wcQzkvBe1NRO3d5_lxiv90LHQVWZR9w0egIl0UEO3nr2ff0k1yKMXPooYcQF7Aye6202xeHUphhN9GLDkWq2PnrQYckrObwpYfOnUzTnuvaGOwUP3HLYB4l5dSc2NmQM4rWjuFj2jZIVnG5UeFjSI0tWWu4BasIoVxHVk0SwfrZboJSfgYKM_R_X1yfbVHoYUVeE_Sb-SiiPzCihGRg-4kwXQQ-8F6L8AH8izayeFs-h8bviCzDQUqlnsfveanIV39XuPa3nRPyy3S0)

* รูปที่ 4 Check Out
```

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


