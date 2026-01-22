### `Get` [{{baseUrl}}/Booking/FindByCapacity?capacity=2]

This endpoint finds a list of rooms based on the specified capacity selected by the employee

#### Request

Parameters:

- Capacity (integer)

Content:
- Room number
- Room requirements
- Room capacity

---

### `PUT` [{{baseUrl}}/Booking/Admin]

Allows the Administrator to update a room in the catalogue, given that a valid administrators employee number is provided

#### Request

Parameters:
- EmployeeNum
Content:
- Room Number
- Room Requirements
- Room Capacity

---

### `DELETE` [{{baseUrl}}/Booking/EmployeeRooms]

Allows an employee to delete an existing booking, given that their employee number matches the number used to create the booking

#### Request

Parameters:
- EmployeeNumber
Content:
- Room number
- Room capacity

---

### `GET` [{{baseUrl}}/Booking/FacilityManagerBooking?EmployeeNum=string]

Allows the facility managers to book a room, or cancel a booked room for maintenance, given that a valid employee number is provided

#### Request

Parameters:
- Employee Number
Content:
- Room number
