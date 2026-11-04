# sre-github-lab
# Clinic Management System

## Overview
Small clinics often track patients, appointments, and visit records on paper or in scattered files. This causes double bookings, lost records, and long waiting times. This project documents the requirements for a Clinic Management System that helps receptionists, doctors, and patients manage appointments and patient records in one place. The intended value is faster scheduling, fewer errors, and easy access to patient history.

## Scope
- In scope: Register a new patient.
- In scope: Book, reschedule, and cancel an appointment.
- In scope: Record and view a patient's visit history.
- In scope: Generate a daily appointment list for each doctor.
- Out of scope: Online payment and billing.
- Out of scope: Pharmacy and medicine inventory management.

## Stakeholders
- **Receptionist:** Wants quick patient registration and appointment booking without scheduling conflicts.
- **Doctor:** Wants to see the daily schedule and a patient's past visits before a consultation.
- **Patient:** Wants easy appointment booking and confidence that personal data stays private.
- **Clinic administrator:** Wants reliable records and simple reports on clinic activity.

## Functional Requirements
- FR-01: The system shall allow a receptionist to register a new patient with name, age, contact number, and a unique patient ID.
- FR-02: The system shall allow a receptionist to book an appointment for a patient with a chosen doctor, date, and time.
- FR-03: The system shall allow a doctor to view a patient's previous visit records.

## Nonfunctional Requirements
- NFR-01: The system shall display search results for a patient within 3 seconds when the database holds up to 10,000 patient records under normal clinic network conditions.
- NFR-02: The system shall allow only authenticated staff to view patient records; 100% of record-access requests without valid login shall be denied.

## Acceptance Criteria
- FR-01: After the receptionist submits valid details, the patient appears in the patient list with a unique ID. Submitting without a required field shows an error and saves nothing.
- FR-02: A booked appointment appears in the selected doctor's schedule. Booking the same doctor at an already-taken time is rejected with a message.
- FR-03: When a doctor opens a patient's profile, past visits are listed with date and notes, newest first.

## Assumptions and Open Questions
**Proposed assumptions** (not yet confirmed):
- The clinic has one location and a small number of doctors.
- Only clinic staff log in; patients do not have accounts.
- Each appointment lasts a fixed time slot.

**Open questions** (need stakeholder confirmation):
- Should patients be able to book appointments online themselves?
- How long must visit records be kept?
- Which patient data fields are legally required?

## Project Status and Usage
This is a documentation-only project. No application code exists and there is nothing to install or run. To obtain the files, clone the repository from GitHub or download it as a ZIP. To view this README, open it in VS Code and use Markdown preview, or view it on GitHub's rendered page.

## Author and Contribution Workflow
**Author:** habiba, Roll No. 521 (Software Requirement Engineering course).
