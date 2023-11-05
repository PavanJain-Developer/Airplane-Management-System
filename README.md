# Airplane-Management-System
A system to manage flight bookings.

Gathering requirements - 

P0 - 

Customer should be able select source airport, destination airport, flight date
List of flight for that date, src, destination , pricing
Seats can have type business,economy, premium economy
Price will be according to seat type
Customer should be able to book seat with type
Customer should be make be able to book the ticket
Notify customer through email, sms

Eg - 

Delhi -> mumbai -> bangalore 
Delhi -> bangalore 

Classes 

Nouns, visualisation

City
Id
cityName

Airport
Id
airportName
airportAbbreviation

Airplane
Id
name

AirplaneSeat
Id
airPlaneId
scheduleId
Seat
SeatStatus
TTL

Schedule
Id
AirplaneId
Src
Dest
departureTime
Arrival Time
Metadata
<<status>>

<<seatStatus>>
	Locked
	Booked
	available

Seat
Id 
Seat number
Seat type

<<seatType>>
Economy
business

<<status>>
Delayed
Cancelled
On time

Users
Id
Name
identificationNumber
Email
Phone

Booking
Id
userId
Src - delhi
Dest - blr
departureTime

Ticket
Id
list<Schedule>
userId
