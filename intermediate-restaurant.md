## Restaurant Reservation App

You're building a restaurant table reserving app that allows users to reserve tables for specified numbers of people. The app will need to show only tables that are available and the times they are available. The app will need to store reservations under a given name with a phone number and number of guests.

What stuff do we need:
Available Tables and their time
Reservations

Reservation Index:
* Timestamp index holding array of table:reservation pairs
    * If table is not in index, then it is available

Reservation Document:
* reservationID: integer
* time: datetime
    * Must be in MM/DD/YY - HH:MM format
* name: string
    * Maximum of 15 characters
* phone number: integer
    * Must be in +1 (234) 567-8901 format
* numOfGuests: integer
    * Max of 15

Table Document:
* tableID: integer
* Reservations: object
    * Must be date-time key holding reservation ID