Sprint 2: Seat Selection

Sprint Goal

Allow users to view cinema seat availability, select their preferred seats, and calculate the total ticket price before booking.

Sprint Backlog

1. Design a theatre seating layout.
2. Display available, selected, and booked seats.
3. Allow users to select and deselect available seats.
4. Calculate the total ticket price based on the number of selected seats.
5. Prevent duplicate bookings and selection of already-booked seats.

Seat Status Description

- Available Seats: Seats that are not booked and can be selected by users.
- Selected Seats: Available seats temporarily selected by the current user. Users can deselect them before confirming the booking.
- Booked Seats: Seats already booked by another user or through a confirmed booking. These seats cannot be selected again.

Expected Increment

A functional seat selection feature that displays the theatre seating layout, indicates seat availability, allows users to select seats, and calculates the total ticket price.

Acceptance Criteria

1. The theatre seating layout must display all seats with clearly distinguishable statuses.
2. Available seats must be selectable by users.
3. Selected seats must be visually highlighted.
4. Users must be able to deselect previously selected seats before booking.
5. Booked seats must be clearly identified and cannot be selected.
6. The total ticket price must update whenever a seat is selected or deselected.
7. The total price must equal the number of selected seats multiplied by the price per ticket.
8. The system must prevent duplicate bookings of the same seat for the same show.
9. If a selected seat becomes booked by another user before confirmation, the system must reject that seat and inform the user.
10. If no seats are selected, the total ticket price must be zero.
11. The seat selection interface must provide clear feedback when a user attempts to select a booked seat.

Testing Scenarios

Test Case| Scenario| Expected Result
TC01| Open the seat selection page| All seats and their statuses are displayed correctly.
TC02| Select an available seat| The seat becomes highlighted as selected.
TC03| Select multiple available seats| All selected seats are highlighted and the total price updates correctly.
TC04| Deselect a selected seat| The seat becomes available for selection and the total price decreases.
TC05| Attempt to select a booked seat| The seat remains unselected and a suitable message is displayed.
TC06| Select no seats| The total ticket price is zero.
TC07| Select three seats when each ticket costs ₹150| The total ticket price is ₹450.
TC08| Attempt to book the same seat twice for the same show| The duplicate booking is rejected.
TC09| A seat is booked by another user before confirmation| The system rejects the unavailable seat and prompts the user to choose another seat.
TC10| Deselect all previously selected seats| No seats remain selected and the total price becomes zero.

Sprint Review

During the sprint review, demonstrate the seating layout, seat selection and deselection, ticket price calculation, and prevention of duplicate bookings.

Collect feedback from users on seat visibility, ease of selection, pricing clarity, and error messages. Incorporate relevant feedback into the product backlog for future improvements.

Definition of Done

- The seat selection workflow meets the acceptance criteria.
- Available, selected, and booked seats are distinguishable.
- Ticket price calculations are correct.
- Duplicate seat bookings are prevented.
- All listed test scenarios have been executed and their results documented.
- Changes are reviewed and committed to the GitHub repository.
