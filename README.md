# Aim/Overview of the practical:
The aim of this project is to develop a user-friendly movie hall seat booking system using
Python's Tkinter library for the GUI and SQLite for backend data storage, enabling customers to
reserve, confirm, and manage seat bookings efficiently with real-time updates and data
persistence.

# Design the GUI Layout for the Booking System

• Create a graphical interface with:
o Entry fields for customer name, contact number, movie title, and show time.
o Labels representing different seat sections (Front, Mid, Back).
o A grid of buttons representing seats, with color-coding to indicate availability,
selection, and booking status.
o Buttons for confirming bookings, canceling selected seats, and resetting all
bookings.
o Display the number of available and booked seats.
• Create the SQLite Database for Bookings
• Set up a connection to an SQLite database (bookings.db).
• Create a bookings table with fields for customer details, movie title, show time,
booking date, and booked seats.
• Ensure the table is created only if it does not already exist.
• Develop Seat Selection Functionality
• Implement buttons representing each seat, initially marked as "Available".
• Change seat color to "Selected" (yellow) when chosen by the customer.
• Allow deselection of seats by clicking again, reverting them to "Available".
• Track selected seats in a list (selected_seats).
• Confirm and Finalize Bookings
• Validate customer details and ensure they are all filled before proceeding.
• Save confirmed bookings to the SQLite database with relevant details (customer info,
movie title, show time, and seats).
• Change seat buttons to "Booked" (red) once the booking is confirmed.
• Update the available and booked seat count.
• Generate a unique booking number using the current timestamp.
• Display a booking confirmation message with the booking number.
• Save Booking Data to a CSV File
• Append booking details to a bookings.csv file for backup.
• Add column headers to the CSV file if it’s empty.
• Implement Seat Cancellation Feature
• Allow customers to select booked seats for cancellation, changing them to "Cancel?"
(orange).
• Revert seats to "Available" (green) once the cancellation is confirmed.
• Adjust the seat count after cancellations.
• Display a confirmation message for successful cancellations.
• Add Reset Functionality
• Provide a reset option that reverts all seat buttons to "Available" (green).
• Clear selected and canceled seats.
• Reset the seat count for available and booked seats.
• Handle Application Closure
• Implement a method to close the SQLite database connection when the application is
closed.
• Bind this functionality to the window's close (X) button to ensure proper closure.
• Test the Application for Edge Cases
• Validate that seats cannot be booked without customer information.
• Ensure that no seat is double-booked.
• Handle cases where no seat is selected for cancellation.
• Ensure saving to both the database and CSV is handled correctly, even with multiple
bookings.
