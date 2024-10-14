## Project Goals

### Capstone: Restaurant Reservation System

- You have been hired as a full stack developer at Periodic Tables, a startup that is creating a reservation system for fine dining restaurants.
- The software is used only by restaurant personnel when a customer calls to request a reservation.
- I deployed both the server [here](https://restaurant-reservation-bwet0n73e-sianglings-projects.vercel.app/dashboard).

## Create a Reservation

The "New Reservation" page (/reservations/new) lets users create a reservation with fields for name, mobile number, date, time (starting from 10:30 AM), and guests. Both the form and server validate inputs, displaying errors if there are issues. Clicking "Cancel" returns to the previous page, while "Submit" creates the reservation and shows it on the dashboard for the selected date.

## Search

The "Search" page allows the user to search for an existing reservation by mobile number. Search input can be any combination or length of numbers. Clicking "Find" sends a GET request to the server, and displays all existing reservations with a mobile number that includes the given combination of numbers. "No reservations found" is displayed otherwise.

## Create a New Table

The "New Table" page (/tables/new) lets users create a restaurant table with a name and capacity (between 1 and 8). Both front-end and back-end validations are in place with error messages. Clicking "Cancel" returns to the previous page, while "Submit" creates the table and adds it to the Dashboard.

## Edit a Reservation

The "Edit Reservation" page (/reservations/:reservation_id/edit) allows users to edit an existing reservation. It uses the same form as "Create a New Reservation," prefilled with the reservation's current details. Validations are applied, and clicking "Submit" sends a PUT request to update the reservation and display it on the Dashboard.

## Cancel a Reservation

A "Cancel" button appears on each reservation card when the status is "booked." Clicking it prompts the user to confirm the cancellation. Upon confirmation, a PUT request updates the reservation status to "Cancelled" and removes the "Edit" and "Seat" buttons from the card.

## Tools Used

- Node.js
- React
- React Hooks
- Express
- Knex
- PostgreSQL
- Bootstrap
- HTML5
- CSS
- Git
