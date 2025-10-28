# 🦷Dentist Appointment Automation using N8N & Telegram
---
Automate dentist appointment booking with N8N workflow and Telegram bot integration.

## Overview
---
This project leverages N8N (a fair-code workflow automation tool) and Telegram to create a seamless automated system for booking dentist appointments. Patients interact with a Telegram bot to request consultations, while the backend workflow manages bookings, confirmation, and updates Google Calendar and Google Sheets for record-keeping.

## Features
---
* Telegram Bot Integration: Patients can book appointments directly via Telegram.

* Availability Management: The system automatically checks available slots and prevents double booking.

* Google Calendar Integration: Once an appointment is confirmed, it’s recorded in the dentist’s Google Calendar.

* Google Sheets Integration: Patient details and appointments are logged for administrative purposes.

* Automated Communication: Professionally confirms appointment status and sends updates.

* Files & Media: See **Demo_Dentist_appointment.mp4** for a full walkthrough, and workflow diagrams/screenshots in the **Output/** folder and **Workflow.png**.

## Workflow
---
1. Request Patient Info: Collects full name, phone number, and preferred date/time via Telegram.

2. Checks Availability: Validates slots as per office hours, consultation duration (1 hour), and required break (15 minutes).

3. Confirms with Patient: Suggests available options if the requested slot is taken or outside working hours.

4. Updates Google Calendar & Sheets: Finalized appointments are reflected in both for tracking and reminders.

5. Screenshots: Refer to images in /Output for booking and confirmation steps (confirmation, database, final booking).​

## Setup Instructions
---

* Clone this repository:

```
git clone https://github.com/Sumit-1988-git/Dentist_Appointment_using_N8N_Telegram.git
```
* Import Workflow to N8N:

Use **Dentist_Appointment_telegram.json** for quick setup.​

* Configure required credentials: Telegram Bot, Google Calendar, Google Sheets, and OpenAI API (optional for AI messaging).

* Update Office Details: Edit prompt messages and office hours as required in the workflow settings.

* Run and Test: Start the Telegram bot and follow the demo from **Demo_Dentist_appointment.mp4**.​

## Visual Workflow
---
Refer to **Workflow.png** for how modules interact.​

## Repository Structure
---

* Dentist_Appointment_telegram.json: Main workflow file.

* Demo_Dentist_appointment.mp4: Demo video.

* Output/: Screenshots of booking stages.

* Workflow.png: Workflow diagram.
