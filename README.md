# SRP Time Ledger App

## Project Overview

The SRP Time Ledger App is a lightweight web-based Clock In / Clock Out application built for SRP Global Consultancy employees and onsite auditors.

The app allows employees to securely log in using their assigned Employee ID and passcode, record their daily clock-in and clock-out time, and capture location details for attendance and operational tracking.

The current version is connected to Google Apps Script and Google Sheets, where all employee login and time ledger records are stored.

---

## Purpose of the App

The main purpose of the Time Ledger App is to provide a simple, mobile-friendly attendance tracking system for employees working onsite, in the field, or across different locations in Australia.

The app helps the business:

- Track employee clock-in and clock-out activity.
- Capture location details during clock-in and clock-out.
- Maintain a central time ledger in Google Sheets.
- Reduce manual attendance tracking.

---

## Current Working Version

The current MVP includes the following functionality:

- Employee login using Employee ID and passcode.
- Employee details are validated from the `Employee Details` Google Sheet.
- Clock In records the employee name, email, date, time, latitude, longitude, and map link.
- Clock Out updates the same daily record with clock-out time and location.
- Current status is displayed as:
  - Not Clocked In
  - Clocked In
  - Clocked Out
- The app prevents duplicate active clock-ins for the same employee on the same day.
- The app requires browser/device location permission before clock-in or clock-out.
- Session is saved locally so the employee remains logged in after closing the browser/app.
- Close App button clears the local session and returns the user to the login screen.

---

## Technology Stack

### Frontend

- HTML
- CSS
- JavaScript
- Mobile-friendly web interface

### Backend

- Google Apps Script

### Database

- Google Sheets

### Location Tracking

- Browser Geolocation API
- Google Maps location link
