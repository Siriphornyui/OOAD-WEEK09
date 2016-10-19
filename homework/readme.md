#OOAD HOMEWORK09
##CLASS DIAGRAM

class1
code

```
@startuml
title Classes - Class Diagram
class OnlineStore {
  +Store
  +Product
}
class Customer {
  +Fristname
  -Lastname
  -Age
  -IDcard
  +Sex
 }
class Address {
  - Rorad
  - City
  - Country
  - Postcode
 }
 class Payment {
  +Cash
  +Tranfer
 }
 class Delive {
  +Post Office
  +Meet
 }
Customer-->OnlineStore
OnlineStore*-right-Payment
Customer*-up-Address
Customer-->Payment
OnlineStore*-left- Delive
Delive-->Customer
@enduml
```


