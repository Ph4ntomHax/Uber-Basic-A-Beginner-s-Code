Uber Fare Simulator in Python
This Python script simulates an Uber ride request, allowing users to enter their desired travel distance and choose between UberBlack or UberX. The program calculates the estimated fare based on distance, ride type, and time-based price adjustments.

How It Works:
The user inputs the trip distance (km).
The user selects UberBlack (B) or UberX (X).
The fare is calculated with a random multiplier depending on the ride type.
Time-based fare adjustments are applied:
Morning (before 12:00) → Discount of 5
Afternoon (before 18:00) → Increase of 5
Night (after 18:00) → Increase of 10
A random driver distance is generated to estimate arrival time.
The program simulates waiting time before displaying the estimated driver arrival.
The user receives a thank you message at the end.
Features:
✅ Random pricing simulation for more realistic results.
✅ Dynamic driver arrival time estimation.
✅ Time-based fare variations.
✅ Error handling for invalid inputs.
