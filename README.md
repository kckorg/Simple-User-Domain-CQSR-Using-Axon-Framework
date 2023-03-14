# Simple-User-Domain-CQSR-Using-Axon-Framework
this simple project describe User Domain that have 3 changes event (UserCreatedEvent, UserActivatedEvent and UserDeactivatedEvent)

UserCreatedEvent   --->   UserActivatedEvent  --->  UserDeactivatedEvent


#Architechture Design
--------------------------              ---------------------                 ---------------------------
CommandUserService                                                             QueryUserService 
(mongodb as event storage)   ------->        kafka                ------->      (redis as query storage)

--------------------------              ----------------------                ---------------------------


