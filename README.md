# Movie Ticket Booking System

## Overview
This is a simple C program for a movie ticket booking system that allows users to:
- Insert movie details (Admin only, requires a password)
- View all available movies
- Book movie tickets
- Cancel booked tickets
- View all past transactions

The program manages movie details and transactions using file handling.

## Features
1. **Insert Movie Details**
   - Requires an admin password (default: `12345`)
   - Stores movie details such as code, name, release date, and ticket price in `data.txt`

2. **View All Movies**
   - Displays all available movies from `data.txt`

3. **Book Tickets**
   - Allows users to select a movie by entering its code
   - Collects user details (name, mobile number, number of seats)
   - Saves booking records in `oldTransaction.txt`
   
4. **Cancel Ticket**
   - Users can cancel a ticket by providing the movie name and their name
   - Removes the booking record from `oldTransaction.txt`

5. **View All Transactions**
   - Displays all past ticket bookings from `oldTransaction.txt`

## Usage Instructions
1. Compile the program using:
   ```sh
   gcc movie_ticket.c -o movie_ticket
   ```
   
2. Run the executable:
   ```sh
   ./movie_ticket
   ```
   
3. Follow the on-screen menu to interact with the system.

## Files Used
- **data.txt**: Stores movie details (code, name, release date, price)
- **oldTransaction.txt**: Stores booking records (name, mobile, seats, total cost, movie name, ticket price)

## Notes
- The program assumes a maximum of 100 seats per movie.
- User input is handled via `scanf`, so ensure valid data is entered to avoid errors.
- Transactions are stored persistently using file handling.

## Future Enhancements
- Implement user authentication for bookings.
- Improve error handling for invalid inputs.
- Enhance UI with a graphical interface.

## License
This project is open-source and free to use.

