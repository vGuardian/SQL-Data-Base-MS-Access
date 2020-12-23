# SQL-Data-Base-MS-Access
Need Help with this Query
I have this problem that where I need to sum more than one column
It Also ask for several column from another table this the problem 
And the code
Colonial Adventure Tours calculates the total price of a trip by adding 
the trip price plus other fees and multiplying the result 
by the number of persons included in the reservation. 
List the reservation ID, trip name, customer’s last name, customer’s first name, 
and total cost for all trips where the number of persons is greater than four.
CODE Query
SELECT Reservation.ReservationID, Trip.TripName, Customer.LastName, Customer.FirstName
FROM (Reservation INNER JOIN Trip ON Reservation.TripID = Trip.TripID) 
INNER JOIN Customer ON Reservation.CustomerNum = Customer.CustomerNum
WHERE NumPersons > 4;
