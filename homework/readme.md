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
diagram

<img src= "https://github.com/Siriphornyui/OOAD-WEEK09/blob/master/homework/02.png ">


class2

code

```
@startuml
title Classes - Class Diagram
class recipient{
   +Fristname
   +Lastname
}
class Address {
  - Rorad
  - City
  - Country
  - Postcode
 }
 class Sender{
  +Store
  +Product
}
class Delive {
  +Post Office
 }
recipient*--Address 
Sender--> Delive
Delive --> recipient
@enduml
```
diagram

<img src="https://github.com/Siriphornyui/OOAD-WEEK09/blob/master/homework/02.png">

class3

code

```
@startuml

title Classes - Class Diagram

class CPU{
   +mainboard
   +ram
   +rom
}
class Equipment{
   +mouse
   +keyboard
   +moniter
   +printer
}
CPU*--Equipment
computer*-right-CPU
User-->computer
@enduml
```

diagram
<img src = "https://github.com/Siriphornyui/OOAD-WEEK09/blob/master/homework/03.png">

class4

code
```
@startuml

title Classes - Class Diagram

class Car{
  }

class Driver{
+Start Car
+Stop
+Speed
+Slow down
 }
 
class Engine {
 +moter
 +batter
}
Car*--Engine
Driver-left->Car

@enduml
```


