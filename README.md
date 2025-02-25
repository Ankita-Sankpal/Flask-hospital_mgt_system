# Flask-hospital_mgt_system
A receptionist in the Hospital Doctor Appointment System manages patient appointments, doctor schedules, and general inquiries. Below is the step-by-step workflow:


---

1. Logging into the System

The receptionist opens the system and enters their username & password.

If correct, they are redirected to the Dashboard.

If incorrect, an error message appears (e.g., "Invalid Credentials").


* Key Points:

Use a secure login system with password hashing.

Display a "Forgot Password" option if needed.



---

2. Viewing the Dashboard

After login, the Dashboard shows:

Today's Appointments (List of booked patients).

Doctor Availability (Doctors on duty).

Quick Actions (Book new appointment, cancel appointment, reschedule).



* Key Points:

Keep the Dashboard simple for quick access.

Use color codes (e.g., Green = Available, Red = Unavailable).



---

3. Searching for a Doctor

The receptionist searches for a doctor by name or specialization.

The system filters doctors based on availability.

The receptionist selects a doctor and views available time slots.


* Key Points:

Implement auto-suggestions for faster search.

Show only available slots to avoid double-booking.



---

4. Booking an Appointment

The receptionist enters patient details (Name, Mobile, Illness).

Selects a Doctor, Date, and Time Slot.

Confirms the appointment by sending OTP verification to the patient.

Once OTP is verified, the appointment is booked and stored in the system.


* Key Points:

Ensure no time slot overlaps.

Use SMS or Email notifications for confirmation.



---

5. Modifying an Appointment

* Rescheduling:

Find the patient’s appointment.

Choose a new date & time and confirm changes.


* Canceling:

Find the appointment.

Click Cancel and enter a reason.

Notify the patient via SMS or Email.


* Key Points:

Rescheduling should be allowed only if the new slot is free.

Keep a log of canceled appointments for records.



---

6. Managing Walk-In Patients

If a patient arrives without a booking, the receptionist can:

Check doctor availability for emergency slots.

Add them to a waiting list if no slots are available.



* Key Points:

Keep a "Waiting List" section to track walk-ins.

Ensure priority handling for emergencies.



---

7. End of Day Reporting

At the end of the shift, the receptionist reviews:

Total Appointments Booked

Cancellations & Reschedules

Doctor's Remaining Slots
