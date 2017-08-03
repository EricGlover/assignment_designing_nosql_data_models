# Needs
* Table
  * seats / space
  * times
  * reservations

* Patrons
  * Contact name
  * Contact number
  * Number of Guests

## Model

```javascript
  Table: {
    seats: Number,
    reservations: [
      Patron: {
        contactName: String,
        contactNumber: Number,
        numberOfGuests: Number,
        time: String
      }
    ]
  }

```
